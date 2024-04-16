---
showLink: "https://www.youtube.com/watch?v=MtNr-Ov78oc"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-building-on-square-with-richard-moot"
title: "Teach Jenn Building on Square with Richard Moot"
publishDate: "2022-08-09"
coverImage: "https://i.ytimg.com/vi/MtNr-Ov78oc/maxresdefault.jpg"
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

[00:00] >> Hello, hello, beautiful humans. Thank you for joining another Teach Gen Tech.
[00:06] Today we have Richard. Richard, please introduce yourself
[00:10] and what we're going to be learning about today. >> Thanks. I'm happy to be here.
[00:16] I'm Richard Moot. I lead our Developer Advocacy Team for Square,
[00:21] which is a block formerly known as Square. Then I also lead an API Design Team within Block
[00:30] to help other teams in designing and building APIs. Today, we're going to learn how to build on
[00:37] Square's platform and all the things that you could do with it. >> I'm pretty excited about this to follow up from
[00:44] Bakari's two episodes and also, for everybody that was getting excited to join right away,
[00:52] I was definitely distracted with learning the difference between the API designs
[00:58] compared to governance and that's a story for another day. But Richard does cool things is what I'm getting into.
[01:06] Where would you like us to start today? Because I do have my dashboard,
[01:12] I got terminal, I got VS Code. >> Awesome.
[01:16] >> I can start wherever you would like. Sharing my screen would probably be helpful.
[01:21] >> Yeah. Let's start there. The one thing I didn't get ready because I was just so
[01:26] excited to ask you a million questions before we went live. I have all three up right now.
[01:34] >> Perfect. We have your application info. I guess my question for you is,
[01:42] trying to build off of some of the things that you were learning previously with Bakari,
[01:48] what would be the thing that you're more interested in knowing about? Maybe we can figure out how to decompose that a little bit,
[01:57] and so learn each one of those pieces as we go along. >> Sure. That is a great question.
[02:07] I'm going to load. It has really quick.
[02:12] I would say something that I got a little, it's just getting changes,
[02:22] so I'm going to load the documents. There we go. I feel like this is breaking it down pretty basic,
[02:31] so bear with me. When we were talking about with his training,
[02:42] it was building the web payments in Next with the React wrapper? >> Correct.
[02:59] >> I think that's where I was getting a little mixed up was, Next is one format and then React is another format.
[03:08] I mean, they're both JavaScript, but they're two different formats.
[03:12] >> Right. >> How does that work?
[03:15] >> Yeah. The tools that you're using is Next.js, which is like a framework.
[03:23] It's actually like a combination of Node.js and React. You think of all the stuff on Node.js,
[03:31] and this is all your back-end style stuff, this is running on the server,
[03:36] and then React is like what is going to be like managing your UI flows and everything.
[03:42] The oddity that you're going to get from using Next.js right off the bat
[03:46] is these things are merged together. Next.js is really almost like using React as
[03:54] a templating engine to display data back to a user
[03:58] as they're navigating through the site. I think that part of that,
[04:03] when you're first learning about React or learning about back-end programming,
[04:09] merging those two together, even for people who are really familiar with React,
[04:14] it can get really confusing because there's all this other stuff like server-side rendering
[04:18] and things where it's like you have to make all these decisions at various points,
[04:23] that I think confuse it. I think one of the things we could do
[04:27] is we can just try to do a basic create React app. I don't know if you've ever done one of those before.
[04:32] >> I have with Anthony. We did a React app with Vite and Vercel.
[04:43] But that was when I first barely started, so I think it was actually like episode number 2.
[04:49] Trying to go back through that by myself was definitely very difficult.
[04:55] I'm not opposed to doing that again because it's like, I think a big part of it,
[05:01] and this is for everybody learning, is being able,
[05:05] especially with coding and learning all these languages, I've noticed that I may not
[05:10] understand everything somebody is telling me first off, but it then starts to make sense once I do it a few times,
[05:17] and then also being able to relate it to something else. By the time I worked with Bakari,
[05:24] I was like, "Okay, this is starting to make a lot more sense." Yet, how to relate what I learned with him to what I
[05:31] learned with creating the React app with Vite and Vercel from episode 2,
[05:37] that's not quite going through. >> Yeah. Let's just pull up your terminal,
[05:43] and are we in the directory where you would be creating new projects?
[05:51] >> I will be shortly. >> Cool. I always like
[06:00] watching how other people organize where all their projects go, because I just have this one projects folder somewhere,
[06:06] and every little experiment I ever do just gets slammed into that folder.
[06:09] >> Yeah. That's something from very, very early on, Ramon suggested that I create a folder,
[06:16] and I'm like, "What do you mean?" He's like, "Code folder works."
[06:21] I'm like, "Okay, that's what I'm going to name it. That is its name."
[06:24] >> Whatever works. All right. We're going to use,
[06:29] let's run a command called, where it's going to be npx,
[06:33] and then space, and then create-react-app. To briefly explain, are you familiar with using npx?
[06:44] I'll give the quickest explanation of this. >> I'm guessing npx is like NPN.
[06:51] >> I get very excited and hit enter a lot, so it might drive you insane.
[06:57] I try not to, but I get really excited. >> I've never done this, so we're going to learn what happens.
[07:01] I'm pretty sure it's going to ask you what you want to name your project because that's
[07:07] the only thing we're missing is naming what we want this to be. >> Yes. I think I did a bit of this with, oh.
[07:19] It's yelling at us, which is fine. We'll run the command again,
[07:24] and then we can go ahead and just name this. While you're running the command,
[07:28] I can give you the quick explanation. Npx is just really a way to immediately run
[07:34] an NPM package that's within the NPM package manager system. For certain tools like create-react-app,
[07:43] create-next-app, and other almost like command line tools, it's really easy to just use Npx.
[07:52] Instead of having to install that package globally and managing a version of it on your machine,
[07:58] you just say, just go fetch it and run it and then ignore it. >> Just to recap, Npx doesn't download it to the machine,
[08:07] it just pulls the information where NPM downloads it. >> Right. Because typically if you ran NPM install,
[08:15] it would try to install it like you're running a node app in this particular directory.
[08:21] Npx is a way to just use a tool that's already hosted somewhere. I think if we're getting really persnickety,
[08:27] it does cache stuff on your machine somewhere. But it's not like you're installing it globally
[08:33] and always running it from command line. >> Got it.
[08:38] >> Cool. Now we just want to change directories to RichardIsRad. Because I haven't actually fixed this yet,
[08:46] I'm just going to, yeah, there we go. >> Cool.
[08:57] >> Then we can just run code and then period, and then that will pop it open in VS Code for us.
[09:04] >> Yes, because that's what I had to just do because it doesn't actually work normally.
[09:10] Every single time I have to redo that first part to tell it to run it,
[09:17] even though I've enabled it a million times, I tried doing it,
[09:20] fixing it based on an article someone sent me and I broke bash. It wouldn't even pull a directory.
[09:28] I'm just manually going to do it. At some point, I will ask someone from Microsoft of how to fix it.
[09:36] >> Yeah. The amount of times that I've had to start wrestling with VS Code is way too often.
[09:43] Let's go ahead and just run this. We can actually go to the terminal and just run npm start.
[09:50] This should pop open your browser, and we can see the basic React app running.
[10:04] All right. Cool. I see that it's running. >> Yes.
[10:08] >> Let's try and just get that React payment form running in the React app. First, let's kill our server,
[10:19] and we're going to run npm install, and we're going to name the package react square.
[10:26] All these are hyphens, perfect. Square web-payments-sdk, web-payments, and then -sdk.
[10:43] This time we have a plural, so we should definitely be getting the correct package.
[10:49] >> It's a fun one, finding that stuff. >> Cool. We can just ignore these vulnerabilities for now.
[11:01] We can just go ahead and get our development server running again. Just npm start, and we'll just let that run in the background.
[11:15] Let's go over to VS Code, and we can start pulling in React square web-payments-sdk.
[11:22] We'll navigate to source or SRC there, and then let's just open up the app.js file.
[11:29] >> Interesting. I'm going to take a moment because this was super, super easy just to install it and use it.
[11:36] I remember the day after that I tried to do it myself, I was like, "Why is this so complicated?"
[11:44] It's not. Apparently, it wasn't clicking yet. All right. Thank you. >> I think you're pointing out something that's really good
[11:52] that I think is important to call it. I say this because being in a DevRel team,
[11:57] I'm very much always thinking about developer experience. One of the things that I always think about with this stuff in particular,
[12:04] is sometimes it's almost too magical, where it's like, "Oh, I just ran this little command,
[12:09] it created this whole thing for me." Then there's a part of your brain that goes,
[12:13] "That was just too easy. I'm missing something."
[12:17] I always think about that when it's like, if you actually have something like do too many things for someone,
[12:22] they start to go like, "Wait, there's something that I'm missing and this is going to bite me later."
[12:28] >> Interesting. >> Thankfully right now, this just gets us in the most basic of a React app,
[12:33] where it's loading stuff, has a functional component there that we can actually start editing,
[12:39] and it'll update everything in real time. >> Interesting. I think that's a great call-out because yesterday,
[12:46] I learned about Bedrock CSS. I believe that's what it's called.
[12:53] It was yesterday, I should probably remember. But it was really cool because Travis taught me how to manually do this,
[13:03] and do all of the web layouts, and then showed me how Bedrock could do it within HTML.
[13:11] It was really cool learning how to do it the hard way, and then seeing how the easy way could work,
[13:16] but I knew how much went into it beforehand. What you're saying of that was too easy.
[13:23] Why was it too easy? >> I feel that way about Create React app a lot of the time,
[13:27] where it's really great for when you just want to put together a UI really quick and not think about all that stuff.
[13:34] But there's a few times where I've had to, there's a thing called ejecting the Create React app,
[13:39] and that basically undoes all of the magic for you, and then you can manually tinker with things.
[13:45] But it's very intimidating when you actually have to look at your full project directory and all of that.
[13:52] >> Yeah, I bet. >> Let's go ahead at the top there,
[13:55] and we'll import some components from the React Square WebPane SDK. We'll just do import,
[14:04] and then we will do some curly brackets. Then we're going to just go past that and put a space,
[14:13] and then quotes, and then React Square WebPayments SDK again. Sweet, autocomplete, to the win.
[14:23] >> WebPayments, there it is, yes. >> Yeah. See, this is where autocomplete is
[14:27] just so clutch because you can't mess it up, because it's actually looking in
[14:31] your modules folder to find the right one. >> Yes.
[14:36] >> Let's put, I think it's probably wanting you to put a colon at the end there, or semi-colon, and then let's go back into those curly brackets,
[14:45] and let's import the, I feel like I need to look up the documentation here.
[14:52] This is probably something that's worthwhile. I don't know. I think I could probably send this to you in the chat.
[15:01] But here is the documentation. >> There you go.
[15:06] >> I just Google it. >> Yeah. Let's show people real coding by Googling stuff.
[15:13] >> Because this one. >> So not that one. You want the-
[15:18] >> This one, right? >> Well, no, we want to go off the GitHub package.
[15:22] So just slightly up there. Then from there, we can get to the documentation.
[15:27] >> This is exciting because I haven't done much in GitHub. Rizal taught me about it,
[15:32] and then I'm like, I haven't touched it because I'm too scared to touch it. >> Yeah. GitHub is great because when you start really tinkering with other packages,
[15:42] you sometimes end up going and reading through other people's code inside of the thing on GitHub to be like,
[15:47] is this actually going to do the thing that I want it to do? If we want to see our docs,
[15:53] so they have a really good read me if we scroll down, but you can see the docs linked on the right there.
[15:57] That's a much nicer setup. So the reason that this is all separate is this is actually a package that was
[16:04] created by one of our community members called Seed, and they basically built this entire wrapper around our Web Payments SDK.
[16:14] It's actually modeled after one that we built ourselves for the, there's a thing before Web Payments SDK for anyone who
[16:20] enjoys the history of payment forms called SQ payment form. Then we deprecated that and now we have Web Payments SDK.
[16:29] Then before we could even build our own React wrapper, these folks built one and it's great.
[16:35] It's modeled exactly how we did our previous one. >> Very cool.
[16:40] >> If we click on the docs there, we can at least have this up and this will help give you
[16:44] a little bit of context of the components that we're going to be pulling in. Then we can also reference any options that we want to mess with.
[16:53] >> Oh, cool. >> We can click on "Docs" and then here,
[16:58] we can see these are all the different components that we have. >> Oh, interesting.
[17:04] >> We've already gone on installation, but we can take a peek at that.
[17:11] This is giving us basically some of the steps we already did. We want to pull in payment form and credit card.
[17:20] >> I felt like I'm being really blind getting started, perhaps credit card. >> Oh, sorry. It's actually like you scrolled past it on the right.
[17:28] >> Oh, thank you. >> Yeah, you can see the steps there on the under fast track.
[17:32] We say, how do I get this up and running? We already did the NPM install,
[17:36] so the next step we want to do is bring in that payment form. >> Okay. Credit card, don't payment form.
[17:44] >> That's the first one, yeah. >> Just to verify, so we always have this in AppJS?
[17:51] >> Yeah, this is the root component of our React app right now. I remember you saying this last time,
[18:00] we're going to try and avoid copy-pasting from the docs into our app. We're going to try and actually write these out so that you feel like,
[18:08] okay, I actually pulled this in. We can go step-by-step on what's going on here.
[18:12] The first one is in those curly braces for React Sql Load Payments SDK. Let's go ahead and type in payment form.
[18:21] That's the one we want. >> Auto install or autofill.
[18:27] >> Then we'll put a comma after that, and then we'll also bring in credit card.
[18:34] We'll just start with that for now. >> Okay, cool.
[18:39] >> Now, I don't know why it's upset with us about, oh, yes, we've got the from. >> Oh, import from, okay, I see.
[18:51] >> There we go. Now, we can go ahead and replace some of these HTML elements inside of that function.
[19:04] Let's go ahead and remove that A, the anchor element, and then let's just put the payment form there.
[19:14] >> It would be the export default function? >> Just below that, we want to put what you see there is like a less than.
[19:26] It's like a bracket and then payment form. >> Okay. I'm catching.
[19:34] Because we have the return up here. >> Right.
[19:36] >> Okay. Then we're not doing- >> If you have questions about what's going on here,
[19:43] feel free to fire them away, and I'm happy to walk through what's going on in the component right now.
[19:48] >> Okay, cool. Thank you. What up, Ben? Ben taught us about web accessibility last week,
[19:55] and we're going to do even more. There's so much learning about the web,
[19:58] the Internet, so much Internet. I think just as a side question of like we right here,
[20:06] it looks like they put export default function app at the top where it looks like it's at the bottom here.
[20:12] Does that make a difference? >> That's more of a stylistic thing.
[20:16] >> Okay. >> You can choose to do it in either place.
[20:21] The important part about that exporting is just it's so that you can pull it in from that file into another file.
[20:31] We actually probably want to move this payment form. >> To underneath the div?
[20:37] >> Yeah, within the div. >> Within the div?
[20:40] >> Yeah. Kind of like where we just deleted the anchor tag,
[20:43] let's just write it in there underneath that paragraph. It's perfect right there.
[20:53] Yeah, we'll just do payment form and then just ignore that thing with the ellipses and the props.
[20:59] >> Okay. >> We can just do a closing bracket.
[21:03] All right, and we hit "Enter", and then let's put in the credit card component,
[21:09] exactly what you just did with the payment form. >> I'm just going to look at it. I'm starting to associate.
[21:15] >> Yeah. >> I think that's the hardest thing is recreating it.
[21:18] I'm like, I'm really good at doing it when someone tells me to, but and then do I do the name of what we called the app?
[21:29] >> For now, we actually, and here's one thing that we want to do is,
[21:33] we want to delete that last credit card one. We're going to do basically like a singular.
[21:40] I don't know how to describe this, but basically you can put a slash at the end of credit card right now,
[21:47] and it will just do space slash. >> Inside of the brackets,
[21:53] and what that does is it basically says this is just like a closed component. It's not going to take in anything within inside of it.
[22:00] It's just a singular thing. >> That's cool.
[22:04] >> You have this sometimes with image, like you can see up above on the image, HTML element.
[22:12] You don't ever put anything inside of an image. It only usually references stuff,
[22:16] and so you can just close HTML element like that. It's a way of just writing a markup language to say,
[22:24] "Hey, there's nothing else that actually goes inside of this thing." >> Ben said we call this self-closing.
[22:30] >> Self-closing. Thank you, Ben. >> Self-closing. All right.
[22:34] >> I knew somebody, just put it out there and the Internet will correct you. >> Yesterday, I was on a Twitter space and I was like,
[22:43] I don't even, we've been talking about this one thing, and I just spaced what it's called.
[22:48] So it's cool. No big deal. Okay, cool.
[22:52] >> I think have we saved? It's probably going to give us a bunch of errors in our React app.
[22:58] >> I did just save. >> Perfect. Let's go back over to your browser
[23:02] and look at what it's going to tell us that we have wrong. >> No, go back.
[23:09] >> Just type localhost. I'm sure it'll want to,
[23:15] it's localhost 3000. Close. What the heck?
[23:20] >> I'm just going to type it. >> Who bought the domain localhost?
[23:24] >> Okay. So it's localhost 3000. >> There we go. Okay.
[23:30] Now, we can open up our DevTools and let's take a peek. I'm pretty sure that we're missing a few props that we need to set.
[23:42] Let's close that what's new in Chrome. Hopefully, you're not needing to know what's new in Chrome right now.
[23:48] >> No. >> If you hit "Escape", we can open up here your console again,
[23:54] and then you just want to close that little x. >> Oh, thank you. There we go.
[24:00] >> All right. So we can see, please contact your developer.
[24:05] Okay. That would be me and you. So we can contact ourselves to find out what's going on.
[24:12] So yeah, I think what we need to do is on the payment form, we need to set our application ID and location ID.
[24:19] >> Okay. Where in here would I have gotten that? Or is that just like you learn it as you go and would have known that?
[24:30] >> I actually just know this. >> Okay.
[24:33] >> So I'm looking at the errors and I'm like, this probably could be a little bit more descriptive
[24:41] in telling us that we're missing some required props. >> Okay. I made the mistake last time of see if it actually does it on the not.
[24:52] No, that's okay. That was looking up locations.
[24:56] So you all can see that. But I got to find them all.
[25:02] SDK, yay. Because I, what?
[25:07] Actually, I'm going to sidetrack myself. >> Sure.
[25:10] >> How did we look it up in here? Because it wasn't, what up, Bakari?
[25:15] Because it wasn't like a known area to find this information. Like it was kind of difficult to find it.
[25:22] What was it again? >> So the application ID and location ID,
[25:27] you can find them inside of that app there. So you already have that one that's Bakari is dope.
[25:31] We can go ahead and use those credentials. From here, that's your application ID right there,
[25:37] and then below that is your access token. >> Okay.
[25:40] >> Yeah. Funny thing is after watching and learning along with you last time, I actually forwarded that on to my designers
[25:49] because I thought it was very interesting that. >> It was so hard to find?
[25:55] >> Exactly. >> Bakari, we made a difference.
[25:59] Then does it say in here where the location is? >> So it's because you have a kind of [inaudible]
[26:25] >> Really quick, is it just me or is Richard breaking up for everybody? >> It might just be me.
[26:35] >> It might be me. My Internet gets a little bit wonky here and there.
[26:40] >> Oh, right. Okay. You sound better, I think.
[26:46] I heard something, something, something, application ID. That's about all I got.
[26:51] >> So we can go ahead and copy over that application ID. So inside of the top payment form bracket,
[27:00] let's press "Enter". >> Inside the bracket?
[27:04] >> Yeah. We're going to put in some new lines and do another one. We're going to keep this well-formatted.
[27:12] We can hit "Tab" and then let's just start typing in application ID. >> I'm sorry, Bakari.
[27:18] >> I sound like a robot? >> No, Bakari said that you two are breaking up.
[27:27] >> Sorry. That was a very, very bad sidetrack, but that was funny.
[27:32] Payment form and what am I doing? >> Let's hit "Tab" and then we're going to type in
[27:41] application and hopefully, there we go. It's going to auto-complete a property for us and we could paste
[27:47] in that and then let's do another new line. We're going to type in location.
[27:56] >> Location ID and then the location was over here. >> Yeah, if you hit that.
[28:01] >> I saw locations, right? >> Yeah, perfect.
[28:04] >> Sweet. >> This is the easy way to find the location in your account,
[28:09] but there is also a locations API, but that's not relevant here.
[28:14] But it's just to mention to someone you can dynamically fetch this information using our APIs.
[28:19] But for now, this is just for us and our integration. >> Is location always needed as often as credentials are?
[28:27] Is it always part of credentials? >> Not necessarily.
[28:33] This is like we're going into how things work with our APIs, but a lot of things are scoped to a location.
[28:41] Certain customers or customers are actually a bad example. Catalog items that somebody might have in their Square account,
[28:48] those are typically scoped to locations. Orders that are created are scoped to a location.
[28:54] Because a single Square seller could have multiple locations, and so we have to make sure that
[28:59] the order goes to the particular location, because that's how they might do their own reporting,
[29:03] and tracking which location is making certain amount of money kind of thing.
[29:09] >> Okay, safe. >> All right. Now, we should have something.
[29:17] >> Oh, we do. >> We got a payment form.
[29:21] >> Yay. >> Cool.
[29:23] >> Then if we wanted to do account, what was the one that Bakari and I did that would do it through?
[29:34] >> ACH. >> Yeah. Now, I just want to see if I can do it.
[29:40] >> Yeah. >> It would be here and maybe.
[29:47] >> Yeah. We can just pull in another component. >> It would just be,
[29:54] would I have to do all of this for payment form then for the ACH, or would I do import of here?
[30:00] >> You just add in that ACH component below the credit card one. >> I'd have to add it into the payment form up here, right?
[30:09] >> Inside of the payment form component that you have below there. But yeah, up here where you are,
[30:15] you just do comma, space, and then ACH, and we can import that.
[30:19] Then just below the credit card. >> Then do the same thing.
[30:24] >> Yeah. You just autocomplete ACH, and then we want to self-closing as well.
[30:35] >> Damn. >> Yeah. There we go.
[30:42] We have our other button for re-doing ACH. >> Probably a little silly how excited I just got over that,
[30:47] but hey, that was exciting. >> Yeah. Now we have this working,
[30:53] or at least it's not working, but we have them rendering.
[30:57] >> Yay. >> Now we need to actually wire this up to get it working.
[31:05] Now working in this case for us is just going to be, let's get a payment token.
[31:10] We need to actually define what to do when somebody clicks the "Pay" button.
[31:17] There's another, we need to define a function. I'm just double-checking because I'm pretty sure it's just card nonce.
[31:29] Let's actually go into the docs under credit card, or actually maybe it's under props.
[31:36] No, callbacks. Yes, that's what we want. >> Yeah, that's not confusing at all.
[31:47] >> No, this is actually probably not correct. The amount of time it's been since I've done this is showing.
[31:55] It is card tokenized response received is the name of the prop. After location ID.
[32:01] If we actually go to the very top again, I probably should orient you into the docs.
[32:06] Click on "Props" there. These are all required properties for our payment form.
[32:13] Application ID, that one's always required. There's certain instances where you technically don't need a location ID,
[32:20] but when you're doing stuff like ACH or digital wallets, I think maybe even gift cards and after pay,
[32:28] you do have to define a location ID because those payments get linked directly to that.
[32:33] In some other instances, we just default to a main location.
[32:37] That's like we're just doing some magic for you to make it easier to take payment.
[32:42] >> I dig it. >> We need to define that card tokenized response received function.
[32:49] >> This one, I'm going to copy and paste because it's going within payment form. >> We want to put it just below where we have location ID.
[33:05] >> We're missing just two closing curly braces. Perfect. If we save that,
[33:18] it'll reload and we can enter in a test credit card number. Just do four and then the rest ones,
[33:27] and then some month and year in the future. Then 1, 2, 3, any numbers there and then any numbers here are fine.
[33:41] >> Pay. >> We click "Pay" and if we look in our developer console,
[33:48] so we could alerted this, but we're going to just look in our DevTools and we should see the payload back.
[33:57] There we go. We have the token object. If you click on "Object" down below and we click "Details".
[34:09] Here's all this info. You can see that we have the billing zip code,
[34:14] the card, the brand, expiration, expiration year, last four. But the thing that's really important is we have that token right there.
[34:23] There's two different things you can use this for. You can use that token to immediately process a payment using our Payments API,
[34:33] or you can actually also use it to store a card for a customer profile to basically use that to be able to charge later.
[34:40] Imagine like in a mobile app, it might ask for your credit card number and then it's stored
[34:45] somewhere and then they just use that to make payments. >> Right.
[34:48] >> That's a functionality we have with our Cards API. Rather than going and building a whole back-end,
[34:56] let's just go play around with API Explorer. Let's go back to the developer dashboard and we're going to
[35:04] try and find our way into API Explorer. >> This one. There we go.
[35:10] >> Let's just expand that out. Then if you go up to the top right under "Docs and Tools",
[35:17] you'll see "API Explorer" there. This is one of our pride and joys
[35:25] of tools for helping developers learn on our platform. I don't know if you've used a Postman before,
[35:33] but imagine this being almost like Postman, but in the browser so you don't need to download anything.
[35:39] Because you're signed in, it is aware of certain things about your developer account.
[35:45] If we go to "Select API", we can go ahead and go to the Payments API.
[35:50] Actually, Ian from Postman is going to be on the show later this month, next week.
[36:02] I really should. I have a calendar, I'm finally updating the calendar,
[36:07] but I just know he's on the docket. There we go. >> You should make a little graphic.
[36:13] Are you using OBS or something like that? You should just have a little graphic that you can pull in and be like,
[36:20] here's the schedule and have it float in and float out. >> That's a good idea. I really
[36:24] need to make a nicer schedule for every month. It's just like I also don't always have them scheduled out that far.
[36:32] >> True. >> Because Teach Gen Tech was a whirlwind
[36:38] of people telling me that I needed content and I need to learn the tech.
[36:44] Within a week of me deciding that I wanted to become a DevRel, I started a show and it's almost two months old.
[36:55] It's been a whirlwind and I'm learning. >> That's pretty solid though.
[37:00] >> Yeah, it's pretty fun. I've met really cool people like Bakari,
[37:04] and Ben, and you, because I stalked Square to try to find who the DevRels were to tag you.
[37:12] >> Yeah. >> Thank you for joining and talking us through this.
[37:16] >> Sure. >> All right. What am I doing?
[37:19] >> Let's change from list payments to create payment. Because what we want to do is we want to take that token that you got,
[37:28] and we're going to use that to make a payment. Let's go ahead and click "Get Token" in there.
[37:32] Let's just go ahead and select your default test account. Now we get to go through the joy of constructing a payment.
[37:42] The first thing we need to do is we need to set the amount of money. How much do we want to charge?
[37:48] One thing I'll call out here is the amount is always going to be in the lowest denomination of the currency in which you are processing a payment.
[38:01] In this case, one thing I will say, you can't do zero. It has to be, I think it's usually like the minimum is 100 cents or like $1.
[38:11] This would be, since your account, your default test account is probably in USD.
[38:16] Let's go ahead and select that. It's going to be the bottom one there.
[38:20] >> Yeah. I'm like, why am I not seeing it? >> Yeah. Then for item potency key,
[38:25] to explain item potency key, this is a precaution to prevent you from accidentally charging multiple times.
[38:33] You could actually run a request with one particular item potency key, as many times as you want,
[38:38] but it'll only ever be processed once. This concept is really important when talking about HTTP protocols.
[38:46] You'll probably come across it at some point where people talk about certain methods being item potent,
[38:52] other methods not being item potent. But this is just a way to say,
[38:57] we only ever want this to run once. We don't want to double charge people and have weird stuff start going on.
[39:02] >> That being said, with this request, and to recap,
[39:09] because the access token was, how am I trying to access?
[39:17] Is the item potency key, is this something that is specific to every single transaction and needs to be redone,
[39:32] or is it something that is reused for everybody? There we go. Words.
[39:39] >> They are supposed to be set in the context of a particular request. There's a whole sandbox show that myself and Shannon Skipper did on
[39:51] our YouTube channel where we basically explored this idea of item potency and try to go through it.
[39:57] But at the basic level, it's like for this particular request,
[40:01] imagine that you have a server and it keeps trying to run this thing. Something happens where the network drops and you're just like,
[40:10] "Wait, I don't know what happened." You're sitting there wondering, "Am I okay to run this again?"
[40:15] Well, with the item potency key, as long as you use the same one,
[40:19] you could just keep running that. Even if you haven't gotten a successful response or your network disconnected,
[40:24] you could just run it again and you're guaranteed that the action, assuming that all your data is correct,
[40:30] will only happen once. It's more just in the context of a particular request.
[40:38] >> Groovy. I just found the video, so that way I can watch that later and learn even more.
[40:47] >> Here is the next thing. We can go ahead and look at that drop-down.
[40:54] Here's a bunch of test values. Remember how last time you were trying to find out
[40:58] all these different test values with Bakari? You were initially looking for the credit card ones,
[41:03] so you do have to look those up. But here we actually provide some.
[41:07] If you wanted to just run a request right now, you can just use this and it'll give you
[41:12] all these different conditions that you can test for. But the source ID field is this is where we're going to put our token.
[41:18] Let's go back to the React app and let's copy that token out of there, that CNON, all that.
[41:26] >> Does it need the CNON part? >> Yes. That's just an identifier to say that it's a relic from before,
[41:34] when we used to call these nonces. Now we just refer to them as tokens.
[41:40] Nonce is just a mathematical term for a one-time use thing, which is what these tokens are.
[41:47] >> Just in this request, especially since I know that we don't want to show our API keys,
[41:56] this authorization is showing our API key. >> Yeah.
[42:00] >> Okay. >> It is showing it right now.
[42:02] Technically, we are exposing your sandbox credentials to everyone viewing on the stream right now.
[42:08] But it's okay. It's sandbox and we can rotate your keys right after this and you'd be perfectly fine.
[42:14] >> Yeah, and I'm not going to use this stuff until I can do web payments or something.
[42:21] >> Exactly. I think technically we have the minimum required in order to be processing a payment.
[42:28] But I do want to show you some of the niceties that we have. Some of them might not actually work because you haven't created data in there.
[42:37] Something like say the customer ID field. Down there, we can actually link a customer to this transaction.
[42:45] If you had customers in your account, you would actually see them as auto-completable options here.
[42:52] This is one of the niceties that we have in our API Explorer. Because typically, if you were using Postman or something else,
[42:58] you would have to go run a list customers request, grab an ID, and then paste it in here.
[43:04] We just have several things to simplify that. Another one, if you go down to location ID.
[43:10] Remember how we had to go look that up and set it? Here, you can see it just automatically pulled it into the dropdown.
[43:17] >> That's fun. >> No need to actually go run these other requests.
[43:22] Now, we have the bare minimum and the extra location ID. Fun fact about the location ID.
[43:30] By default, we'll always process a payment on a main location. But here, we want the payment at this particular location.
[43:39] But you only have one. Let's go ahead and run that request. >> That was really hard. I really wanted to click the button.
[43:46] I'm like, "I can't click the button until he says I can click the button." >> Then, you've now made
[43:52] your first payment with your Square account in Sandbox. If we open that up, you can actually see all the info that you get back.
[44:02] Oh, cool. This will actually show you another fun tool. This is our API logs.
[44:07] This is in your developer dashboard. This actually just shows the request that you just run.
[44:14] As you run requests in Sandbox or production, we will actually create logs in here for you.
[44:20] You can go back and be like, "Wait, I did something weird.
[44:22] What just happened? I didn't keep that." You can actually just go back in here and look at what you did.
[44:28] If you click on that, you can actually see what you sent Square. >> That makes sense.
[44:37] Does it only do it from what we just tried, or does it create that API log from what Bakari and I did last week?
[44:50] >> I think last week, you never actually got to the point of making a successful API request.
[44:56] >> I did. >> Then, let's actually change your filters here.
[45:00] We can actually look back and see what happened. >> Because I hard-coded the key and it worked.
[45:08] >> Let's look at the last 28 days. There we go. You can see all of these.
[45:14] This isn't your first payment. You've done some payments.
[45:18] Now, we can actually look back and see everything that you ran previously. >> Sweet. Because I was being a weirdo after that,
[45:25] and I spent four hours on a Friday night trying to figure it out. That's where I got it to work.
[45:34] >> Yeah. Awesome. Another thing, if we go back to API Explorer,
[45:40] this is just another fun thing I want to point out. If you scroll up,
[45:44] you see how we have, that's a cURL request that's actually formed on the right there.
[45:48] But if you click that drop-down where it says cURL, there's a little arrow there.
[45:53] We can actually change that to any of our other supported SDKs. If we click Node.js,
[45:59] you're going to get some example code about how to actually do this using Node. >> Really quick, and this is something that I was getting stuck on,
[46:09] and then also Bakari just said, you can also run these calls from your CLI.
[46:13] Is this the type of thing, and from my Googling and not understanding cURLs,
[46:19] but is cURL something normally, is this area that we're at right here,
[46:28] would this be something someone would put in their VS Code or they would put into their CLI?
[46:37] >> Typically, if you're running cURL, it's going to be from the CLI.
[46:41] I will say that there are some exceptions to that. I think PHP as a language,
[46:47] in some instances, boils down to using cURL. But I would say the majority of the time,
[46:54] you could probably just ignore that fact, running cURL is something you would just run in
[46:58] your terminal to test things out. >> But everything else up here,
[47:03] would that be in terminal or would that be in VS Code? >> This is all part of the cURL request.
[47:08] I can even break down some of those things. The -x, that's just saying the method of the request,
[47:14] and then all those -h's, those are setting headers on the request.
[47:19] It's pinning it to the square version, it's setting your authorization credentials,
[47:24] and then it's also specifying the content type. That -d is to indicate
[47:29] the data that you're actually sending in the payload. >> I'm letting this sink in because I feel
[47:37] like this is something that I wish I understood when I worked at Stoplight.
[47:41] Because it was like I could see this kind of stuff happen with the API designs,
[47:46] and they did have a few of these tests. But I'm like, I don't understand what this all does.
[47:51] This is magical. >> Yeah. All of this is like HTTP protocol stuff,
[47:57] that there's your endpoint URI, the path, the main base URL.
[48:05] But yeah, so if we switch to Node.js, you actually have pretty much a copy-pasteable example
[48:12] that you could put in for running your backend stuff. You probably want to just change a couple things here and there
[48:19] for dynamically say setting the source ID, and the idempotency key in your code.
[48:24] But this gets you 80 percent of the way there. >> Oh, this is happiness.
[48:31] This is exciting. Okay. Thank you. >> You're welcome.
[48:36] >> All right. >> This kind of helps us separate out the frontend and the backend,
[48:41] because everything that we have up here, this is just your frontend stuff.
[48:44] That's the communication of how you start securely capturing payment information from a buyer.
[48:54] We always use this term like buyer and seller. In the case of a buyer,
[48:58] we want to be able to securely capture all that payment info, and you as the developer,
[49:03] you never want to actually be touching that. I mean, some people do,
[49:06] but because they might work in like FinTech of some kind. But the whole reason for all of this is like,
[49:14] when you're using that payment form that we provide, that's creating a direct way for people to enter that info.
[49:22] Like that's just going straight to our servers in an iframe. >> Okay.
[49:26] >> Other things that you might be running in your application can't even see what's inside of that iframe.
[49:32] You can imagine it's almost like we're opening up a tiny little window inside of somebody's browser and saying,
[49:38] "Give us this information directly to Square." Then when you hit the "Pay" button,
[49:43] it's basically sending a message to us to say, "Hey, can you go ahead and tokenize that and give me this token
[49:49] that will represent the information that a buyer just entered?" Then you then can take that token to
[49:56] any like our Payments API or Cards API and say like, "Okay, now do something with
[50:00] that payment information that you got earlier." That's like the high-level explanation of how all this stuff
[50:08] works and why it's secure and why we insist on going about doing it this way.
[50:12] >> I feel like that's really helpful. Also, Bakari, you totally knew the next question I was going to
[50:19] ask or at least look up at some point was Crash Course on the HTTP requests.
[50:26] I do want to say, if anybody knows someone that
[50:29] wants to come on and talk about protocols, just all the protocols,
[50:33] all the different protocols, what are they for? Why do we use them?
[50:36] What are the differences? I would love to have that conversation with someone
[50:39] because coming from the GoDaddy realm of email and stuff like that or domain names,
[50:48] it gets a little foggy trying to put it into API terms. Anybody who want to come on,
[50:53] please send them my way. I would appreciate it.
[50:56] >> Just even somebody going through the entire journey of a request from the very,
[51:02] very, very beginning all the way to the end where it's like, okay, you put in a URL,
[51:07] it's going to go to a domain name server, it's going to do a lookup,
[51:10] and then it's going to find the correct IP address of the thing that it is that you're looking
[51:14] for and then do the translation. It's nutty, like the actual journey
[51:19] of a request and how HTTP works. >> See? I bet you know people, Richard,
[51:24] or Bakari will, or Ben will, or somebody will. Please send them my way.
[51:29] I want to learn this and I bet other people want to learn this too.
[51:32] >> Totally. >> I feel like we've done a lot.
[51:34] Do whatever our next step. >> That's a good question.
[51:40] What else do we want to learn about? I want to try to be sure that we're
[51:48] exploring the curiosity that you have around this. >> I feel like it's at a good point,
[51:55] so that way something I would like to do and follow up on it, would be now that we've taken a look at their Git,
[52:11] and then we went to WeRC and having their documentation too.
[52:18] I myself would want to figure out how to get the pop-ups like we did with Bakari,
[52:24] but it's something that I'm learning that I want to figure out by myself,
[52:29] not with someone necessarily talking me through it, which is really cool compared to two months ago.
[52:35] Thank you, Ben, for saying that earlier. It has been an amazing two months.
[52:39] It's something that I'm actually starting to find things that I want to figure out
[52:44] myself instead of going, I don't know. But I think something just
[52:50] before we wrap up today and going back, you mentioned that a lot of people will go into GitHub to be
[52:58] able to check out the code to see if it matches up what they're doing.
[53:03] Could you guide us on, because I've seen this before.
[53:11] I can get to someone's Git. That was funny for me, nobody else.
[53:16] I know everybody else is over that. But once I'm here,
[53:21] I'm like, I don't know what I'm looking at. I know that Anthony will be on later
[53:27] this week to teach me about reading the READMEs. I know I need to do that.
[53:32] But if you were to come in here and you're stuck on something,
[53:37] what would you look at? >> That's a good question. Part of it
[53:41] depends on what I might be stuck on. First thing I would probably scroll down and just start
[53:46] scanning the README to see if there's any common troubleshooting tips that they might have.
[53:51] You could actually just display it right below the repo there. But we could also look directly at the page.
[53:57] >> Oh, yeah, they do. >> Yeah. They put this here so we can see
[54:01] the docs and the changelog. I might go past the install
[54:05] because I'm probably past that point. You can maybe look here to see the example usage.
[54:11] See, did I miss something in what they have here? Then if we're lucky on a GitHub repo,
[54:17] they have common troubleshooting things, things that people commonly miss.
[54:22] It doesn't look like we have anything here. The other place that I would start
[54:27] looking for if I'm having a particular problem, if you go to the very top,
[54:32] you can actually go into the "Issues" tab. There's two different things.
[54:37] There's issues and then there's discussions. It doesn't look like there's any discussions,
[54:40] so we can go look at issues. We can see here's the things that people are running into and
[54:45] they're hoping that somebody who manages this repo can resolve. I'd probably start by searching in
[54:51] here for the things that I'm running into and see if, if the best situation is that it's an issue that's closed and
[55:00] there's a resolution somewhere within that thread that we can use and maybe use that as a workaround,
[55:05] or it's closed because there's a PR somewhere waiting to be
[55:10] merged to fix the thing that we're running into. >> Okay. I think that does answer a lot of it.
[55:22] >> Now, if you want to know, let's say I know that this library,
[55:28] so here's one thing is like the React score web payments SDK, it is doing a little bit of magic for us in
[55:34] terms of handling web payments SDK. One thing is React renders all of its stuff at a particular pace,
[55:44] but our payment form that we actually provide for the web payments SDK, that actually gets loaded onto the page,
[55:51] but it loads in asynchronously, which means that you don't want it to block the rendering of a page,
[55:58] so it's going to load after the fact, and so usually you want it to load after a particular event.
[56:04] Sometimes it might be like DOM content loaded or something like that. They had to write into the React thing here,
[56:13] when to actually render the payment form, because it needs to have a check to be like,
[56:19] hey, did we load the square web payments SDK yet? Then waits until that happens,
[56:26] and then tries to render the rest of the React code that you're wanting to run. If I was wanting to learn how to do that asynchronous loading thing,
[56:35] I might start looking through the code in here for something to be like, oh, maybe they have a place where they're doing this,
[56:41] and then I can use that to learn how to asynchronously render my React app. >> I know I'm probably throwing a bunch of things together.
[56:52] >> No, it's making sense. In theory, I'm not,
[56:59] just trying to see if I can compare with, we had Mishko on the show a while ago,
[57:09] and he created AngularJS and just launched quick a while ago. Is it something that the web payments SDK
[57:21] could be wrapped in quick instead of being wrapped in React? >> Yeah. The web payments SDK can be wrapped for EmberJS,
[57:33] quick, Angular, VueJS. This is one of the things that I think is
[57:41] the most powerful thing about open source software, is that if you just know,
[57:46] well, they have to be doing this particular thing to make this work, and maybe I just want to be able to do it in the framework that I like using.
[57:54] You can still go look through their code and be like, how are they doing that?
[57:58] Then just be like, oh, that's how they're doing that because at the end of the day,
[58:02] this is all JavaScript. We could just look through it and be like, okay,
[58:06] let's just adapt the way that they're doing that into our open-source package and do this asynchronous rendering and whatnot.
[58:16] >> So much knowledge dropped. As I said, it's starting to make sense the more and more I do it.
[58:23] Thank you for helping fill in some of the gaps that I wasn't remembering from last time or breaking it down a little bit.
[58:31] I definitely feel like there's more I can build upon this, and also it makes a lot of sense on building the React app at this point,
[58:43] just by itself without Vite and Vercel, which I think I need to go back to that at some point,
[58:50] yet it's not as scary just building a quick web app as I thought it was at one point.
[58:57] >> Yeah. I agree because when I was first learning JavaScript, I was in a similar situation of learning a lot of Express.js,
[59:08] React at the same time, and it gets harder and harder to parse out where everything is supposed to be.
[59:15] There's been this convergence of tools of like, let's just have everything in the back-end.
[59:22] Then you're like, wait, but what is the front-end? I feel like you just made this really murky,
[59:27] and I'm trying to understand the difference between what I'm seeing in the browser and what is running on the server.
[59:34] Because that used to be a little bit more clear when you'd be like, "Oh, I just had this Express thing running in the background in one terminal,
[59:40] and then I have what is running over here that's rendering my front-end." You had a much clearer separation,
[59:47] but with Vite.js and Vite and all those other things, everything is on the server and you just have one set of logs,
[59:55] and you get a little bit more confused like, where's the error actually happening here?
[59:59] That's why I like to separate out, learn, create, react app stuff,
[60:04] and later go and learn Next.js and Vite, and all that stuff to understand how that merges in.
[60:10] >> That totally makes sense, and I'm putting in the comments really quick of a lot of what we looked at.
[60:23] Now, I really want to put this in there, but it's API Explorer.
[60:31] I feel like if I link this, people can find it, even if they're not logged in.
[60:36] >> Yeah. I would definitely like, here's my shameless plugs, developer.squareup.com.
[60:41] You can find all of our stuff, our documentation. It has links to all of our community stuff.
[60:47] I also want to plug the fact that we have a Slack community. It's fairly active.
[60:53] I don't know what counts as very active, but there's people in there all the time asking questions,
[60:57] getting help, trying to solve problems in their implementations. Then we also have forums.
[61:04] Don't need all URLs, just go to developer.squareup.com. I'm sure you could end up finding them in the nav under our community stuff.
[61:12] Anybody who's wanting to build on Square, all of our resources should be available to there.
[61:18] >> Agreed. Thank you, Bakari, for starting us off on this journey because I got Richard on here.
[61:26] Thank you, Richard, for breaking a lot of this down. How long has the API Explorer been there?
[61:32] I just want to play on that now. >> Yeah. That's been there for a few years now.
[61:39] >> Okay. >> But we've had some nice improvements here and there.
[61:41] We can just keep finding these little. It doesn't feel right to call them little,
[61:46] but just like these little quality of life improvements of automatically pulling in test values and your location ID.
[61:54] But each one of those has suddenly been more and more powerful. Even now, it'll remember some of your requests that you ran before,
[62:03] and some of the data there. When you come back, you can actually not have to be like,
[62:07] let me go reconstruct that entire request. It also has a feature that lets you create a shareable link.
[62:14] You'd be like, I'm going to send this link to someone else, and it'll fill out all the data that I had for them,
[62:20] with the exception of your access token and other sensitive stuff. But it allows you to just say like,
[62:25] hey, this is what I'm trying to run, and then you can share that off,
[62:28] or you can even save that link in your notes somewhere to be like, I'm going to come back to this.
[62:33] >> This is just happiness. This is so fun. Anyway,
[62:38] I do like that you told me to switch to create payment. Even now, I just went in there and I'm like,
[62:44] it doesn't look the same. Because I need to copy. I can copy that.
[62:52] >> Yeah. The thing that I love about it from a developer experience perspective is it does exactly what it says,
[63:00] which is it allows you to explore APIs, but it also shortens the distance between
[63:04] your exploration phase and implementation. It's one thing to create,
[63:10] and I don't want to be like, this is not a knock on Postman at all, but you go through, you run all these requests,
[63:14] and you're like, okay, I figured out how this thing works. But then you're like, now I have to go write
[63:19] the code that does the thing that I was just tinkering with. That small little step of like, hey,
[63:25] you can copy, paste this code that's on the right here. You're now just that much closer to
[63:31] going from your exploration to your destination. >> Agreed. Even just copy and pasting it into something else like this.
[63:42] This is pretty legit. I'm digging this. I am digging this. I do feel like it's something that does make it a lot
[63:49] easier to understand and mess with. I'm looking at it on another screen and incognito, so sorry.
[63:59] I was getting distracted there since you told me that it's shareable. Thank you once again for being on the show today.
[64:06] >> Thanks for having me. >> As a heads up, probably down the road,
[64:09] I'll be hitting you up again because that's the cool thing of learning about this stuff is it's ever evolving.
[64:16] It never ends, ever. Thank you so much and the video will be uploaded right after this.
[64:26] Everybody, make sure to check it out. Thank you, Bakari and Ben for joining today.
[64:32] We will talk later this week. Bye all. >> Bye.
[64:37] [BLANK_AUDIO] 
