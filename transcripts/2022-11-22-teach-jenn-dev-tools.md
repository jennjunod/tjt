---
showLink: "https://www.youtube.com/watch?v=NQcSFfuaQk8"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-dev-tools"
title: "Teach Jenn Dev-Tools"
publishDate: "2022-11-22"
coverImage: "https://i.ytimg.com/vi/NQcSFfuaQk8/maxresdefault.jpg"
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

[00:00] >> Hello, beautiful humans. Welcome to another episode of Teach Gen Tech.
[00:06] Today we have Nick here. Nick, what are we going to be talking about today?
[00:12] >> We're going to be talking about browser DevTools. We'll be looking at the browser DevTools
[00:20] in a Chromium-based browser, but these tools also exist in Firefox as well.
[00:24] There's some DevTooling in Safari as well. It's not as feature-rich yet from what I've seen.
[00:31] But if you have Firefox as well, we can take a peek at that if you want to too.
[00:35] But yeah, there's so much in browser DevTooling, so it's going to be like a whirlwind tour.
[00:43] But hopefully, some of the things that we look at, they can be hopefully helpful
[00:48] to folks that are checking out the stream. There's just a lot of cool stuff you can do in it.
[00:54] I've seen it happen multiple times when I'm either pairing with somebody
[00:58] or in my virtual coffee community, I mentioned something and they're like,
[01:02] "What? You can do that?" We're just going to take a peek under the hood of what
[01:09] browser DevTools can give us to help us be better devs potentially, or at least give us more tools to see what's going on.
[01:16] >> Yay. Thank you. What up, Ben? What up, homie? >> Very good people.
[01:24] >> Yes. Y'all, I'm pretty excited about this because I did not realize
[01:32] that I somehow have invited three Netlify people on my stream without realizing it.
[01:40] They were all for very different reasons. The only person that we're actually ended up
[01:49] talking about Netlify was Jason. >> Yeah. Well, I can give a shout out. Here you go.
[01:55] >> Yay. Oh, that's cool. That's a good one. That's a good one.
[01:59] All right. I know that we talked about getting another browser.
[02:05] >> Yeah. If you want to go ahead and share your screen, you can just open up, I don't know what you use for your browser,
[02:14] whether it's Chrome or Edge. I'm using a newer browser that's Chromium-based called Arc,
[02:20] still in invite-only mode. Who let the dogs out? There we go.
[02:27] >> Ma'am. Okay. She needs to make an appearance. She's back there being a very, very sassy pants.
[02:34] >> That's all good. >> She doesn't decide to do that the entire stream.
[02:40] Hello, Jay. >> Well, I'll tell you a funny story.
[02:44] Because I used to work at Dev too, like I was telling you before the stream.
[02:48] I used to stream with my coworker, Christina Gordon. She's working at AWS now,
[02:54] but she lives in Costa Rica. Her kids were always trying to break into her office during the stream.
[03:04] But also, because she lives in Costa Rica, there's lots of animals there, including sloths.
[03:11] Then we had one stream and she's like, "Sorry, I got to go for five minutes.
[03:17] There's a sloth in my driveway." We took a sloth break.
[03:22] I filled in while she was gone. But just like all that says,
[03:26] one of the reasons why I like streaming is because it's expected that it won't be perfect.
[03:32] Whether you're live coding or your audio goes off, I know you've been streaming for a while now.
[03:38] I know when I first started streaming, I'm pretty extroverted, so I'm comfortable just talking to people.
[03:45] Even though I can't see anybody aside yourself. But the things that would stress me out are like,
[03:50] is the audio working? Is the video working?
[03:53] Because I'm by no means an AV person, so I know minimal stuff.
[03:57] I remember in the early days of my streaming, the audio was just not working and I had no idea.
[04:04] I'm trying to be all cool on stream. "Yeah, just a minute."
[04:08] Those are the things that stress me out. But I've got a lot of that stuff automated now.
[04:14] So, which we can talk on a tangent later about that if you want to. - Yes. - Because I know you're interested in that stuff.
[04:20] Like, there was so much automation that Jason talked about. I'm like, "Dude, that is so cool."
[04:25] Yes, please, because that is definitely. And just for everybody listening and tuning in,
[04:33] because y'all know about it. And this is Nick's first time on the show.
[04:39] I run late for everything. And so, yes, today I ran late as normal.
[04:43] And I forgot my tea somewhere. I couldn't find it.
[04:45] So, I was just like, "You know what? We're just not going to worry about it.
[04:48] It's just not going to happen today." But, all right, I have my browser.
[04:54] And the only bit of browser, console, DevTools stuff that I've done that I specifically remember
[05:04] is doing the, with Quick, when seeing just like the network side of things
[05:14] and how quickly it was loading. But that was like my fifth stream.
[05:21] So, I didn't know what I was doing. And Caitlin, for the follow, yay.
[05:28] So, I know it's like, is it inspect? - Yeah, so that's how you can start off.
[05:37] Yeah, I guess the Google main page is, let's go to like, well, this isn't a webpage,
[05:45] but let's go to, I don't know, something like the Canva home or the Twitter or something,
[05:50] wherever you want to go. So, like you did there,
[05:56] like we'll start off with some basics here just for folks who might be new to using the DevTools.
[06:01] So, there's a few ways you can open them. You can do what you just did there,
[06:04] which was you right clicked and you said inspect. And then that inspects the current element
[06:08] that you selected. There's also browser shortcuts you can use.
[06:13] You can do, if you're on a Mac, you can do Command + Shift + I,
[06:17] and that'll open up the browser DevTools. If you're on a non-Mac computer, Linux or Windows,
[06:23] you can do Control + Shift + I. It might not be set up.
[06:29] Your mail shortcut might be set up to do that. It's possible.
[06:34] Yeah, I think you're set up with that for some reason. I think I might've turned that off on my,
[06:37] but also depending on other shortcuts, you can use F12 to open it.
[06:45] If you don't have your F keys set up, 'cause F12 by default on Mac is set to volume.
[06:51] - Yeah, I was like, I don't think I have these. I don't know.
[06:54] - Yeah. - Yeah. - But the, yeah, exactly.
[06:57] We can go look at that after, but because we're gonna talk about debugging
[07:03] some JavaScript at some point, and using the F keys to debug through things,
[07:08] like stepping through code is handy. You can use the UI as well,
[07:12] like clicking the play button or the next arrows and stuff, but yeah, so let's open up the browser DevTools again.
[07:19] - And y'all, this is a big reason that I asked Nick to be on the stream
[07:25] is I hear this term debugging. Debugging, it's a thing.
[07:32] It is a thing. - I don't know what it is.
[07:36] - Yeah, so I mean. - In like general idea, I'm like,
[07:39] oh, you go find issues and try to fix them. I think that's what it means.
[07:44] - Yeah, well, yeah, the term debugging just means, I don't know, I've said this multiple times to people,
[07:50] but being a dev is like being a detective, you know, you're just trying to crack the case,
[07:55] you know, like what's going on. So debugging is kind of like a set of skills,
[08:00] but there's actually something in terms of JavaScript, and not just JavaScript, but other languages too.
[08:06] Like you can have an actual debugger, which is something that allows you to go into the code.
[08:11] You can actually stop the program. You can see like, what's the current state of things like,
[08:17] okay, what's this variable set to you and so on. We'll definitely get to that stuff too.
[08:23] But yeah, we're gonna kind of ratchet it up a bit, I guess we'll start off slow
[08:30] and then we'll just kind of dig into stuff. And there's so much stuff in here, like I was saying.
[08:35] So it's kind of gonna be like a whirlwind tour, but if you do have like more questions
[08:41] outside of what we cover, definitely drop me a message or hit up Jen after.
[08:47] I'm just dropping my website here. You can pretty much find me in all the places on there.
[08:53] And I still don't know how I snagged that domain name, but that's another thing.
[09:02] But yeah, oh yeah, sorry, yeah. Can you zoom in the console, Jen?
[09:10] So if you, yeah. - Let me kick the dog out really quick.
[09:13] BRB, BRB. - Yeah, no problem. Yeah, so BRB, BRB.
[09:22] I don't know if, is there a dog command? I don't know, Ryan.
[09:24] Let me see. - There is, I don't know if it's a dog command
[09:30] or a Kiona command. - Okay, okay.
[09:32] I just have the Twitch chat open. - Yeah, I feel like we should do a dog command.
[09:38] Oh, there we go. It is, okay, cool.
[09:41] - Cool, cool. Yeah, no, I'm not looking at the video of Twitch.
[09:43] I just have the pop out of the chat, so. - Oh yeah.
[09:46] - I see Anthony is here too. - Okay, let me zoom in, maybe.
[09:54] - Yeah, like just a command plus a few times if you want. Yeah, perfect.
[10:01] Okay, yeah, and you can make the DevTools the biggest part. So a few things before we even start looking at the DevTools.
[10:08] So I mentioned a few shortcuts, how you can open them. There's also settings.
[10:13] So if you click on the little cog icon at the top right, it's two to the left of the X.
[10:19] So there's a few things here. Some stuff's a little newer.
[10:22] It's been around for a while, I think, but you can do theming too.
[10:26] So like you can have custom themes with an extension, but if you go to the theme there,
[10:30] you can choose light or dark. I'm typically on dark, I think.
[10:34] There's a few other things in here that are helpful too. Whenever I'm working on a website,
[10:43] in the past, I used to run into caching issues all the time because like you're editing something
[10:50] and you're not seeing the changes. So there's actually a very useful feature in the network.
[10:54] On the right there, it's the fourth checkbox down. It says disable cache while the DevTools are open.
[11:02] So what this does is if you don't have the DevTools open, your site's behaving with whatever normal caching,
[11:07] but if for some reason you just don't want the cache happening, you can have that checked off.
[11:12] And I have that on by default. There are times when I actually need to test
[11:16] if something's actually caching, so then I'll uncheck it. But in general, I have that set.
[11:22] So there's a bunch of settings in here, but that's just one I like to have on.
[11:28] Oh, cool, Anthony started a new job in January. Awesome, man.
[11:33] You're going to have to tell me about that. - Yeah, I was like, it's, you guys are popping over there,
[11:39] like chatting a lot. I'm excited 'cause, and it's like everybody
[11:44] that's been on the stream before hangs out with us often, so I'm excited.
[11:49] And yay, Anthony! - It's a reunion chat. - Yeah, congrats, Anthony.
[11:53] Okay, so all I'd say, there's like a ton of settings in here. I'm not going to go through all of them,
[11:58] but that's one that I do like to have on. So we can go ahead and close that
[12:01] if you just click on the X on the top right there. And we'll go through some more, some other basic things too.
[12:08] If you click on the three dots just to the left of the X in the top right of the DevTools, there's a three dots icon.
[12:15] - I was like, I was thinking where it was. I'm like, you said words, it's not clicking right now.
[12:21] - So I typically like to have the Browser DevTools at the bottom.
[12:25] I have a bigger screen, so you can do that. But if you click on those three dots again,
[12:30] there's many ways you can have them. You can even have it pop out.
[12:33] So if you click on the first one, which is the two squares, it pops it out in a separate window.
[12:38] And this is just really a preference thing, so like you might like it popped out,
[12:44] you might like it to the right, to the left. So it's just, this is just kind of warming up
[12:50] with the DevTools. Just kind of showing you like how you can lay things out.
[12:54] - Yeah. - Okay, cool.
[12:56] So we've got that now. So now let's go into Canva,
[13:02] like let's right click on what will you design today there. And just in the actual website.
[13:08] So like if you just, yeah, right click inspect, it'll bring us to that element, which is down there.
[13:15] So a few things to take a peek at. You'll see that it's using Flexbox.
[13:21] So it's got this little pill icon, it says flex beside the div there at the bottom.
[13:27] And if you click on that, you're gonna see all of a sudden it gives you this outline
[13:32] and shows you how the flex is set up and stuff. So this could be handy if you're just trying to see
[13:38] like how things are laid out. We're gonna talk more about the CSS stuff
[13:42] on the right there in a bit. But for now, if you go to the display flex,
[13:49] which you see in the first CSS class there, you're gonna see there's like six little rectangles
[13:54] beside the word flex on the far right in the other panel. - Oh, you know what?
[14:00] I'm gonna pause this really quick. And that's not what I meant to go to,
[14:04] but go to my website actually, because that'll help me understand
[14:09] because the way Squarespace has stuff set up. And then also because we talked about wanting to build
[14:18] the website with like Netlify and stuff like that, that just kind of like seeing
[14:23] what some of the differences are and how stuff is built. So that's not what I wanted.
[14:28] - Yeah, so you can make your browser as big as you want there
[14:35] and maybe zoom in the DevTools again, just once, I think. We'll see what people say in the chat there,
[14:43] but I think zooming it up one more will be good. Okay, so yeah.
[14:48] So let's inspect hello, beautiful human there. So you're gonna see it's got the elements selected.
[14:54] Okay, you have one with flex there. Let's click on the flex one there, just like four above.
[14:59] Okay, so now if you look on the right there in the styles, if you make that panel on the right a little bigger,
[15:05] if you just stretch it out. - Brittany's saying maybe if I pop it out.
[15:10] - Yeah, sure. - It can make it a little easier.
[15:14] So give me a moment. - Yeah, sure, no problem. - Switch it up some.
[15:20] What is this fast scrolling thing that's not stopping? - It's a new feature.
[15:26] It shows you the full thing that's selected, I think. - That's awfully annoying.
[15:33] - So the website itself doesn't need to be that big, but we can stretch out the browser dev tools a bit bigger
[15:38] and maybe zoom in one more time in the browser dev tools. Yeah, if you just come out.
[15:49] Yeah, okay, perfect. Okay, so let's select that flex thing.
[15:52] - Yeah, this is fine. - Yeah, so like you see, it's got a border
[15:58] and that can help you show what the layout is. But if you go into the bottom part,
[16:02] if you stretch up the bottom panel a little bit and find the CSS class that has that flex,
[16:09] it's one of the classes in here. I'm not sure which one.
[16:13] If you scroll down a bit, there's, okay, there. So page section where it says display flex
[16:19] in the CSS class there. It's the bottom CSS class in the panel.
[16:24] So you're gonna see beside display flex, you've got this little icon with six rectangles.
[16:31] So if you click on that, all of a sudden you can start, you're like, say you're new to flex
[16:37] or even if you already know flex, you're just like, it's not doing what I wanna do.
[16:41] You can literally start clicking and these are all the flex properties
[16:44] for that particular class or that particular element that's using this class.
[16:50] And you can just start clicking on those things to say like, okay, what's it look like this?
[16:53] What if I change the column direction to, you know, to a column, sorry, flex direction to column
[17:00] instead of row and stuff. And I think in this particular case,
[17:03] you only have one thing in there, but if you had something with more than one item,
[17:08] you would see these things happen. So you could see it, like if it,
[17:12] by default flex direction is row. So it would be one after the other and it can wrap.
[17:17] But if you wanted to have flex direction column, they would be stacked kind of.
[17:21] So this is just like a handy little tool for you while you're in the browser to go like,
[17:27] okay, well, let me try this out and see what this looks like and stuff.
[17:31] And once you're like, okay, that looks good, you can actually highlight,
[17:36] you can select the entire CSS class there. Like if you just click and drag like the contents there,
[17:43] like even though they're checkboxes, if you highlight the whole thing,
[17:46] and then you could go ahead and paste that back into your stuff if you wanted to.
[17:51] So it's kind of like an in-place way to kind of, you know, have some fun with the CSS there
[17:58] to kind of figure out how you want to have things. You can also add new properties in there too.
[18:03] So like if you click, yeah, exactly. So you could just, I don't know.
[18:06] - Wait, I didn't mean to do that and it did it. (laughs)
[18:11] - It's AI, it's a GitHub Chrome pilot or something. I don't know. - Oh, okay.
[18:17] - But you could, like, for example, you could say background dash color,
[18:21] and then you could say red, for example. And if you want to add the actual value,
[18:27] you just click tab once you're done, and then you can type red,
[18:31] or you've got a list already, so pick whatever. And you're gonna see, once you click out of there,
[18:38] it should change it depending where it is. You might have other stuff that's the CSS specificity,
[18:44] so it might actually not do it, but basically you can come in here
[18:49] and you can start editing the CSS that way too, which can be interesting.
[18:56] The other thing is, we'll get back to inspecting the elements in a bit,
[19:00] but since we're in the CSS stuff here already, if you bring the DevTools back to focus here,
[19:07] so we have the styles, like if you look in this panel, you'll see at the top it says styles,
[19:12] computed, layout, et cetera. So styles are what classes
[19:16] or what CSS rules and properties are there. But say you're like, okay, I set my page section color
[19:23] to paragraph medium color that you're variable there. You're like, why is that not showing up?
[19:30] So like, for example, let's see if we can add, let's see, what can we add?
[19:39] Well, let's go first to the computed tab, which is the one beside the styles.
[19:43] So here, there's a few things. You can kind of see the layout,
[19:46] so it shows you like the margin, the border, the padding, and then the actual content and stuff.
[19:52] But the thing that's important to note here is on the bottom, you're gonna see all the CSS properties
[19:57] that are set on that particular element. And so like, say for example, the background color,
[20:03] which is some kind of reddish orange right now, you're like, why is it that color?
[20:08] You know, like I set my background color to blue or something.
[20:12] If you click on the arrow beside the background color on the left of it,
[20:16] it's gonna open up a little details panel. Oh, sorry, not that arrow.
[20:21] But that arrow actually brings you to where it's actually set.
[20:25] - Okay. - So that's also good too. But if you click on the arrow beside it here, yeah.
[20:30] - Yeah, okay. - So you're like, so like say, 'cause there's something
[20:34] called CSS specificity. So some things can override what you actually set
[20:39] 'cause they're more important. So you're like, okay, why is my background color coral?
[20:45] And then when you open that, it shows you why it's that color and where it is.
[20:50] Because you could have like two competing styles set. And for whatever reason, one is winning over the other.
[20:58] And this is CSS specificity. If you folks wanna Google that,
[21:01] if you're not familiar with it, but I can drop a link to that if not.
[21:05] So this is a good way to see like, okay, this is the actual style for this particular element.
[21:11] And this is why these things are being set this way. And like you did with the little arrow before it,
[21:17] if you click on page section, I believe it'll go to it again.
[21:22] Yeah, so it's got the arrow there. - Okay, so there's two different ways, that's cool.
[21:26] - Yeah, so what you could do is, so right now you see there's a color in page section
[21:33] and then you have another class and then there's a section. And so you can see a couple of things here.
[21:42] I'm trying to see if we can add something to just kind of demonstrate this,
[21:45] but you should be able to add just a style to the element. Like if you scroll up in that panel.
[21:52] Okay, yeah, yeah, go right to the top. Okay, yeah, in element style.
[21:59] So element style is like, this is gonna be something that's called inline style.
[22:03] So let's add a new property in here and let's just say color is yellow or something.
[22:10] This is a terrible color. Well, yellow on black is pretty good for accessibility,
[22:16] but pick anything, honestly. - I was like trying to figure out why yellow wasn't there.
[22:22] And then I realized I was like, cause I need to scroll. - Okay, and before we go back to check that,
[22:29] or we can come back to it after, but you see how there's the little yellow square
[22:32] beside there, if you click on that, you can actually start selecting colors with a color palette.
[22:37] And these are all things that are built into the browser. These aren't browser extensions.
[22:42] This is native to the browser dev tools. So you can do that that way,
[22:47] or you can actually put hex numbers in. You can also change it to,
[22:50] if you click on the two arrows there, not there. If you check that again and you click on the box,
[22:58] there's two little arrows there, yeah. - Oh.
[23:01] - And then you can change it to RGB, RGB. Like these are just different color formats
[23:05] depending on what you prefer. Hex is pretty common still, but RGB is used a lot too now.
[23:11] Cool, so, okay. All right, so what we've done here now,
[23:17] if we just click out of here, you're gonna see that the color is set
[23:20] to some kind of teal or aquamarine. And we still have our color.
[23:25] If we scroll down in your page section CSS class, you're gonna see color.
[23:31] Okay, right away you can see color is, it's crossed out. - Oh yeah, in page second, yeah.
[23:37] - So this is because of CSS specificity. The style we set up top there
[23:41] when you added that aquamarine color, that's an inline style
[23:46] and that takes precedence over a CSS class. So if we go to the computed now,
[23:51] like say you're like, why is my paragraph medium color not being picked up?
[23:56] Click on the color here and you're gonna see why now. If you click on the little arrow to the left of the color,
[24:02] you're gonna see, oh, well it's, is it not opening?
[24:07] Okay, it's getting, or if you click on the arrow, oh, it's 'cause there's no CSS class.
[24:10] Click on the arrow and it's just gonna bring you to, and the reason why it's this color
[24:14] is because we've set it in line and that's why the other one isn't set.
[24:18] So this can be helpful when you're having CSS specificity issues.
[24:22] It's very difficult to say that specificity. I think Wes Boss, whenever he says it,
[24:27] he always calls it specificity or anyways, it's like a running thing.
[24:32] - I'm like, I'll probably butcher it so I'm not even gonna try.
[24:35] - Yeah, I'll, let me just find real quick a link to CSS specificity 'cause there's some fun games,
[24:43] like there's a Star Wars reference, but I'll link to the actual MDN here
[24:49] that folks can check out if they wanna, if they wanna read up more on that.
[24:54] But basically there's rules. So like, and like inline style
[24:58] is usually the one that wins out on everything. There's also like, if you add a exclamation mark important
[25:05] on something that can make it more important to you, there's a whole set of rules.
[25:09] But if you check out, yeah, it's a game, Brittany, that's right.
[25:13] But if you check out that MDN post I put in there, it'll explain it well.
[25:18] Okay, so yeah, so that's the kind of neat stuff in there. - See it very quickly, go for the link, all right.
[25:29] - Cool, now, if you come back to your website, so let's go, when you hover over one of your links,
[25:35] like your shit you don't wanna talk about, does it change? Okay, it doesn't, okay, you don't have a hover or anything.
[25:43] Okay, I'm trying to think if, okay, let's go to my site for a second,
[25:48] not 'cause I'm trying to promote it, just I know it has links that change.
[25:53] So-- - .com? - Yeah, so if you hover, don't click on the links,
[26:00] but in the latest post there, if you hover over one, you're gonna see it, it gives an underline.
[26:06] So say you're trying to figure out like, okay, I'm hovering on it,
[26:09] and then I wanna go to the dev tools. So like, if you go to the dev tools now,
[26:13] like, yeah, you can inspect it. You're like, okay, I'm in the,
[26:18] okay, that's one thing that's also different. If you pop out, you're gonna have the dev tools.
[26:22] - You'll have so many, and what have 10? - So one thing here is like, say I'm like,
[26:28] I wanna see what the style is, like when I hover over this thing,
[26:32] but you just went to go inspect the element, and now you don't see my hover effect.
[26:36] So what you can do is, that's selected now. If you click in the CSS styles panel to the far right,
[26:45] the fifth icon, the colon H-O-V, which means hover, you can actually enable things.
[26:52] So you can, if you click on the hover, you'll see it's gonna underline it.
[26:56] So you can actually debug or like change what your CSS styles look like for when you're hovering
[27:01] while you're in the dev tools. 'Cause because of the nature of it,
[27:04] you're not hovering it over it because you're in the dev tools.
[27:07] This allows you to say, hey, put it to hover mode so I can see what the styles look like,
[27:12] or if I wanna tweak them and stuff. And you can do this for other element states too.
[27:18] So active is kind of like when somebody's in the process of clicking on something.
[27:22] So it's like the mouse is still held down or a keyboard action's happening.
[27:29] If something gets focused, you can, if you click on the focus,
[27:33] it should give a focus ring, I believe. Yeah, you see it.
[27:37] So these are just interesting things to allow you to debug your CSS, which can be super helpful.
[27:44] So that's another panel in there. There's also, if you click on the .cls there,
[27:52] just to the side of it, you could add other classes to it.
[27:56] So I can't think of any at the moment, but if you wanted to add another CSS class
[28:03] in the CSS classes you have available, you could actually just start typing in one
[28:07] and it would add it to the HTML for that particular element. Cool, okay.
[28:15] We can go ahead and close my website 'cause we don't need to promote it.
[28:18] It's your stream, so let's get back to your website. No, like yours, how did you build yours?
[28:25] What is everything built in? Maybe like, talk me through,
[28:28] like if I were like, hey, you have a really cool site, I want to go build my site like your site.
[28:34] - Okay, cool, cool. I do want to show one thing though.
[28:36] If you stretch the site out to make it a little bigger, it'll change.
[28:41] There you go, you get an alpaca. - Yay.
[28:44] - So my site's built with Eleventy, which is a static site generator,
[28:49] but it also does server side stuff now too. But I was using Gatsby a long time ago.
[28:56] And honestly, the only reason why I was using Gatsby, this was back in 2017, was I was doing React
[29:04] and then I was at a job where I wasn't doing React. So I was like, even though it's not a good reason
[29:09] to make a website, a blog in React necessarily, I was just like, I'm just gonna use it
[29:16] so I can just still keep learning React. But I didn't do much with it.
[29:21] And then, it's had a few iterations. When I worked at Dev2, we had this integration
[29:28] with a company called Stackbit. So you could actually write your blog posts on Dev2.
[29:33] And then the Stackbit integration would actually deploy a site to Netlify.
[29:38] That's who they're partnering with. It's not just 'cause I worked there.
[29:41] And at the time I had chosen a Gatsby template and it would just basically update my posts and stuff.
[29:48] But then I got off that and then I found Eleventy at some point.
[29:52] This is, again, before, yeah, did somebody say Eleventy? Yeah, exactly.
[29:56] - Yeah, Ben, I totally went to go grab, 'cause look how cool Ben's is too.
[30:01] And Ben-- - Ben has a badass site, it's super cool.
[30:04] - I did not realize this, but without meaning to, I apparently just wanted to channel my inner Ben
[30:09] and have the same colors. - Yeah, no, I love Ben's site.
[30:15] It's just, I don't know about yourself, even though, like I was telling you before,
[30:20] I was the lead front-end at Dev2 before, but I can take designs and I can do it,
[30:26] but I'm the same person that, I'm not a designer, and I'm the kind of person that will spend a week
[30:32] trying to figure out what font I should use. Like, that's me.
[30:36] But if you give me something, I can definitely produce it. - Yeah, this is something that I'm wanting to,
[30:45] I'm thinking about because I'm like, oh, I need to go build my site,
[30:48] and so it can do automations. 'Cause even as we're going through this,
[30:52] like we're talking about like how, just to compare just something that I had a hard time
[30:58] figuring out that I want to make sure others see is, especially with Jason's stream last week of saying like,
[31:06] I am a developer, I built a Squarespace site, there are plenty of people that don't know
[31:10] how to build a Squarespace site, is the customizations that can be done
[31:16] and going through and even using the dev tools, that's why I was like, yes, let's stick to your site.
[31:21] Because in Squarespace, you can't do as much. Where with yours, like we were even already able
[31:29] to see a lot more, so. Oh, yeah, putting it in Figma first, yes.
[31:37] At least you do that, I just will try to start building. - 'Cause you were asking about automation,
[31:43] I'm gonna drop a couple of links that I wrote about for automating things.
[31:50] So let me just drop those, give me two seconds here. Because like I was saying, I do use Eleventy
[31:59] and that should be both of them, yeah. Cool, yeah, so I do use, what's that?
[32:09] - Oh, I just said yay, thank you. - Okay, cool, yeah, so I do use Eleventy
[32:13] and then basically the StackBit integration with Dev2 got phased out, I don't know,
[32:21] I can't remember why, but I think Stack, I don't know, for whatever reason, it got phased out.
[32:26] So like for about two months, I was literally copy pasting Markdown from Dev2
[32:31] into like pages that I was creating by hand. And then three weeks before I started at Netlify,
[32:39] I was like, I have time off, I'm gonna automate this. So I finally wired it all up
[32:45] and it's the first post I talk about that I dropped there. So I use the Dev2 API to pull in my posts
[32:52] and then I generate the Markdown and then it pushes to my GitHub repo where I host my site,
[32:59] excuse me, and then that deploys to Netlify and it just, 'cause that's all automated.
[33:06] Like when you have Netlify attached to a repository, it'll just deploy it as soon as you push stuff there.
[33:12] - And then- - It's just exciting. I was just like- - Yeah, no, it's super cool.
[33:15] - There's so much that can be automated. - Yeah, no, and it's honestly like,
[33:21] it takes a while to get there. Like I was telling you before the stream,
[33:24] like even my own stream, like I have these silly things, like I have an alpaca on my stream, it hides,
[33:29] it changes hats, you can move things on the screen. But when I first started streaming,
[33:34] it was literally my webcam in the corner of OBS, a black screen and DS code or a browser and that was it.
[33:41] And it's like, it's only been over time that you build these things up
[33:46] and you also learn from other streamers, like Jason Langsdorff or just speaking to other streamers,
[33:53] like how do you do that? Or like, 'cause I couldn't find a lot of stuff and then,
[33:58] so yeah, there's, but getting back to the automation, I'm pretty happy with my flow now
[34:04] because I'll write a blog post on Dev2 and then I have a GitHub action
[34:10] that fires every night around 8 p.m. Eastern. And then it'll check, do I have any blog posts?
[34:16] If there are, or if a blog post was updated, it updates it. And then that, I have another GitHub action
[34:22] or maybe it's the same GitHub action. It creates a pull request and if all the checks pass for it,
[34:28] like it basically does a deploy preview of Netlify. If all of that passes, then it automatically merges itself.
[34:34] So I never have to do anything. So it's, I'm pretty happy with the flow.
[34:40] - I definitely wanna look into GitHub actions sometimes. And also just in like the way that I like found out
[34:51] about what Jason was doing and what you're doing, I'm like, what if I have the schedule that's posted
[35:00] and autopost on all social media for me? So it's not me going, oh shit, I never scheduled that
[35:08] and having to automate it. The way that Jason was talking about that with Cloudify.
[35:14] - Oh, Cloudinary maybe for his. - Cloudinary, yeah, yeah.
[35:19] - Yeah, 'cause he generates the social, I can't speak, social images.
[35:26] Like, so like the card you sent out with the picture of you and me.
[35:29] So that's what he's talking about, Cloudinary. So there's that part.
[35:33] And then I guess he's probably hooked up to like the Twitter API, LinkedIn or where,
[35:37] I think he only posts it to Twitter at the moment. But yeah, there's a lot of stuff you can do.
[35:45] And once you get those things in place, you also have to wanna do it.
[35:52] Like I just hit a tipping point where I was like, I have enough time, I'm just gonna do this.
[35:56] And it's also interesting to do 'cause you're learning stuff.
[35:59] Like even for my own stream, like I don't post to social media automatically.
[36:04] I do that by hand, but I have like my guest info on my stream and that, I used to do it manually,
[36:12] but it's happened a couple of streams where I forget to change the guest info.
[36:15] And so it's like, it's this, yes, we're here today with Jen Juneau.
[36:19] And then on the bottom it says, John Doe from some other company.
[36:24] So I'm using Airtable now to pull in that data. And I'm actually using, not to promote Netlify,
[36:31] but I'm using a Netlify edge function and it basically pulls in the data from Airtable
[36:36] and then it renders the page with that information. So I never have to do anything.
[36:40] So now all I have to do is make sure that the Airtable has the proper information
[36:44] and that's all I have to do. And that saves me time
[36:47] and it also saves me from making mistakes. And the same thing with like,
[36:53] I didn't have one for the longest time, but I have one of these now, I have a--
[36:59] - Oh, hold on, hold on, let me make sure. Oh, I was gonna, so you can put stream decks on tablets.
[37:07] So I got this tablet to work on some Android stuff. So I'm gonna put the stream deck on here,
[37:15] but I'm still super lost on OBS that I have not done this yet.
[37:19] But I wanted to say, I saw in passing, yes, Anthony, we all just steal from each other.
[37:27] I 100% agree. That's kind of just like art in general.
[37:31] Art in general is you literally just steal from each other and recreate in your own way.
[37:37] But there was something else that you said that I was like, that is so cool.
[37:42] Oh, also the auto-generating in, I need to set up Netlify.
[37:48] And as a super, super side note, y'all, I have two mods that show up like all the time.
[37:57] Oh, sorry, yes, I have ads set up. I wanted to see if it can make money.
[38:02] I'm still officially looking for a job. I have to go do it.
[38:05] But anyway. - Right, stop talking.
[38:08] Jen is looking for work. If you're hiring, hit her up.
[38:12] She's streaming all the time. I think you blogged too.
[38:15] She got your website, so hit her up. - I do blog, I do.
[38:17] - What are you looking to do? Are you trying to get back into DevRel
[38:20] or you want to be an engineer? - Yes, yes, I love streaming and talking to people
[38:24] and working with people. It's always so much fun.
[38:28] And it's definitely something, yes, I want to get back into that and job hunting,
[38:35] but getting OBS set up to do all of these things, I'm like, that is like such a good way
[38:40] to finally look into getting more into like Netlify and building my own site
[38:48] instead of my laziness of Squarespace. I say laziness because I didn't really know
[38:53] what to build with. And Jason, okay, Brittany, I'm really glad you're here
[38:58] because Jason asked me this last week and Anthony, you're here.
[39:01] So like all like the like people that have been here for a long time.
[39:07] So I'm debating, should I build my new site in Nuxt because I emcee Nuxt Nation?
[39:15] And if I could do more stuff with Vue, like I'm gonna see if I can maybe be like the Vue emcee
[39:22] for in Amsterdam. I'm like, I feel like I just need to focus on a language,
[39:28] but I'm like, what if I just focus on that because that ended up happening.
[39:32] - Yeah, there's that. I'd also throw out there's Astro
[39:37] and you can actually pick what component library you wanna use.
[39:43] So you could actually use Astro and write it all in Vue. That's another option.
[39:49] I'm not saying don't use Nuxt. I've never used Nuxt.
[39:52] I did one stream on Vue with my buddy, Drew, but it wasn't Nuxt or anything.
[39:59] It was just like Vue out of the box, but I've heard good things about Nuxt.
[40:03] And I know Nuxt 3 is, I think it came out recently and you can deploy that to the edge now too.
[40:11] I think that's stable. I'm not positive about that, but Brittany says it best.
[40:15] Just pick something, you know, like it's kind of like when people are saying like,
[40:19] I should start blogging and then they'll be like, okay, but I got to build my site first.
[40:23] And then all of a sudden you're completely derailed. So it's like, it's a separate thing,
[40:29] but like if you're gonna blog and like, say you don't have a website set up right away,
[40:33] you know, use something like Dev2, Hashnode, just start blogging.
[40:38] And then when you get around to it, you know, bring that into your own site or start bringing,
[40:43] 'cause you can, they all have APIs, so you can bring in that stuff,
[40:46] or you can literally just copy paste it into your own site. But I would say probably go for something automated
[40:53] just to make your life simpler over time. But honestly, just start writing.
[40:57] So like, it doesn't matter where you post it. Like Ryan's saying he likes Hashnode.
[41:02] Obviously I'm slightly biased towards Dev2 'cause I used to work there,
[41:05] but I post to Hashnode as well. You know, just get your content out there.
[41:09] And, you know, I think long-term having your own site, like owning your own content is super important as well.
[41:17] And you'll hear a lot of people say that. Yeah, Brittany uses Dev2.
[41:21] I know a bunch of the Netlify team has a Dev2. Since Netlify people are here and,
[41:27] oh, not what I meant to click, Jesus. Okay, that scared the bananas out of me.
[41:31] Oh, jeepers. So this is a Hashnode thing.
[41:38] And I was like, dude, this is like the coolest thing ever, that it plays the article for you
[41:44] and it makes it more accessible. And I was just like, I wanna do this.
[41:51] Yeah, you could. So, but can it only do it on Hashnode
[41:56] or is it something like, this is something that can be built for anything?
[42:00] This is, I think, where I get also paralyzed with. And as I can add that to my own site.
[42:09] - Yeah, so that's a built-in feature of Hashnode. But also just a side note for if you're using a browser,
[42:17] a lot of them allow you to just, you can go into a reader view,
[42:20] but you can also play audio, like on my phone's my camera right now,
[42:24] so I can't show it. But like, I use the Edge browser on my phone.
[42:30] And like, I go for walks at night and like, I'll listen to podcasts and stuff.
[42:35] But sometimes if there's an article I wanna read, you can actually just click play article.
[42:39] It's not even in the website. It's like the browser itself allows you to read it.
[42:43] And then- - Because I use, we've-
[42:47] - Yeah, there you go. - BitBeef, but I use Natural Reader,
[42:52] I think is what it's called. - Okay, that's an extension.
[42:55] I'm not positive if it's built- - Yeah, here it does it for mobile too.
[42:58] - Okay. Yeah, I'm not sure if the desktop browsers have it built in.
[43:02] I feel like they do, but it's definitely on my mobile one. But this is a complete side note.
[43:09] And I think Ben Myers is still here. Playing a website to listen to it
[43:15] is when you're gonna feel the pain of somebody who has accessibility issues.
[43:22] If the website is not built correctly, it's gonna be like, it'll start reading,
[43:27] like I was listening to an article the other day and like the first three minutes,
[43:29] it was reading like so much irrelevant stuff. And then it finally got to the article.
[43:36] But so it's an aside, but basically it's really important
[43:41] to make your site accessible. And that's why, you know,
[43:45] there's people that trash talk HTML saying it's not a real language and all that stuff,
[43:48] you know, the haters on Twitter. But, you know, these are people typically
[43:52] that I think haven't put a lot of time into it. You know, the people that say like HTML
[43:57] and JavaScript and CSS are easy. It's easy when you put like an alert,
[44:01] you know, background color red and like a small piece of markup.
[44:05] But like to make really good websites, it takes a lot of effort.
[44:11] And semantic HTML is really important there. That's why you always need like a main section.
[44:17] You want something called like a skip link so that you don't have to necessarily
[44:21] go through like all the navigation. You can just use the skip link
[44:24] and it goes right to the main section and stuff. And I know we're not talking about DevTools at the moment,
[44:29] but it's an aside, but. - Yeah, like I feel like this is the fun part
[44:33] about streaming is it is a very conversational and y'all have the people
[44:41] and Nick, I feel like you're going to be like wrapped up into this too.
[44:44] You're just going to have to come on the show again. - Oh yeah, that's cool.
[44:47] (laughs) - 'Cause like everybody here has,
[44:51] almost everybody has been on the show multiple times, but to the mods, thank you for all that you do
[44:58] because Ryan and Homie, they set up all the clicky clicky things.
[45:05] And then also keeping the conversation going when we don't have anybody here.
[45:12] So I just want to say thank you. - Cool, cool, awesome.
[45:15] Yeah, shout out to mods. I know it's not easy.
[45:17] I worked in community, like DevTools, like DevTools has about a million members now,
[45:23] like active members and like moderation is like, it's huge. Like we have a lot of volunteers.
[45:30] I mean, there's a dedicated team too, but moderation is not easy
[45:34] and you got to stick to your guns. - Yeah.
[45:39] - Yeah, I was going to say Ben Meyers shared a link to skip links from his blog.
[45:44] Definitely check everything Ben writes about Accessible, anything Ben writes is really good,
[45:48] but I definitely encourage you to check out the skip links. It's a super useful thing to add
[45:54] and it's not that difficult, honestly. And it's saying, it's true that,
[46:01] Anthony's saying it's true that the article was inspired by a random convo in a street.
[46:06] Ah, cool. - I dig it.
[46:07] That's kind of like the best way to have it done. And yes, y'all, sometimes I forget that my,
[46:16] when I don't share my screen, that it's not sharing. There, again, yes, everyone,
[46:26] because we did go down like a total rabbit hole, but going back to taking a look at these sites is they,
[46:34] y'all just teach me so much and it's about all of it. And also just on being able to think about accessibility,
[46:45] because as you're developing a site, it's so important. And I feel like it does really go in a full circle
[46:53] because to use DevTools, I'm guessing a lot of it is to check up on sites
[47:01] and to build a site, you need to look at all of this. So it does help.
[47:06] - No, it's a good segue to get us back here. We can even go to Bensite.
[47:12] I really love the look of Bensite. And we can close the DevTools.
[47:18] Yeah, if you go ahead and close the DevTools over there, just 'cause it's gonna open up a different one for Bensite.
[47:23] And so if you just inspect anything here again, and we'll kind of.
[47:28] - It's like doing a very random one. Whoa, what did you do?
[47:33] - There's a CSS selector to allow when you select something. So I'm assuming they're changing just the background color.
[47:43] It's a nice look versus the default. But yeah, so if we go ahead and.
[47:51] Yeah, so if we go ahead and inspect something again here, and we were talking about accessibility and there you go,
[48:02] there's the accessibility panel too. This is something that definitely accessibility experts
[48:08] and people who've been doing front end for a while probably know about,
[48:11] but for people that are new to web dev or even just the DevTools,
[48:16] let's go ahead and click on the accessibility panel here. So what this does is you're gonna see this view here,
[48:25] and you're gonna see like banner and you see it says, howdy, I'm Ben.
[48:29] So what's happening here is banner is a type of role for an HTML element.
[48:35] In this case, I believe it's an H1 that the howdy is, but you can see, okay, so this is important to see
[48:42] because like when a screen reader is reading, it's gonna say something like heading, text, howdy, I'm Ben,
[48:49] and then keep going on and stuff. So like this is super, yeah, sorry, it's header,
[48:54] not H1, I think, yeah. Oh, and thanks for dropping the accessibility tree too.
[49:01] Ben's my co-pilot today. So this is super important
[49:06] because when a screen reader is actually going through a site, so say you have a form,
[49:11] I don't know if, Ben, do you have a form on your site, like a contact page or something that we can maybe look at,
[49:18] or if not, we can just find some site with a- - Nope.
[49:24] - Okay, that's just regular, okay. So we could go to, let's just-
[49:28] - I have a form, I have a form, be a guest. - Be a guest.
[49:33] Okay, so let's go here. Okay, now let's inspect here.
[49:36] You're gonna get another dev tools open. Okay, and let's go back to the accessibility tree here.
[49:44] And let's have it so that, let's shrink your browser a bit, but let's have it so we can still click
[49:50] on the form elements. And so let's inspect the first one that says
[49:54] where you have the placeholder text, Gen Junod. - Yeah.
[49:58] - Is it Gen Junod or Gen Juno? - Gen Junod, Juno, like it's almost like,
[50:05] it's said so many different ways, I don't even care anymore.
[50:11] - But what is the real way, 'cause I'm always mindful of how you say somebody's name.
[50:17] - Well, since I started in the API world, there are many, many, many, many French humans,
[50:25] and it should said Juno, and- (speaking in foreign language)
[50:31] - No. - Okay, all right.
[50:34] - No, and my mom says it Junod, so I just go with what she says.
[50:43] - Okay, yeah. - But eventually, yes, one day I will learn French,
[50:47] one day. - Okay. - One day. - Yeah, I know.
[50:50] Well, I'm in Montreal, so it's bilingual, and I've been doing French since kindergarten,
[50:56] but yeah, it's a lot of, there's a lot of French names in the States
[51:02] like that get Americanized, so like, I don't know, like Leclerc or something,
[51:09] that's like Leclerc in French and stuff. It's like they get rid of, I don't know,
[51:15] they just change them, but anyways, I just wanted to know how you said your name, that's all.
[51:20] - But did y'all know that Avocado for Deverell is because it's also like that in French,
[51:31] is it's like very, very close? Let me see.
[51:35] - Yeah, it's Avoca. - Yeah, so it sounds like Avocado.
[51:40] - Yeah, you spell it like this. The funny thing about it is that that means avocado,
[51:44] but it also means lawyer in French. I don't know if there's any joke there,
[51:47] but if there is, somebody make it. - Okay. - Anyways.
[51:54] - So we got the form, we got the form going. - Okay, so let's, okay, let's look at,
[52:00] we can see in your markup here, so you have a label element on the right there,
[52:06] and you have an input. And I can already see that there's,
[52:11] you have a for attribute on the element, like if you look in the dev tool,
[52:15] so it says label for equals some UID, it looks like UUID.
[52:21] And then that's the same ID as the input. So already this is good semantically,
[52:26] and it's accessible because the label is tied to the input. And so now like when you go to the text box
[52:33] in the accessibility tree here, you see it's called name,
[52:35] and it's called name because the label's linked to it. And that's super important,
[52:40] because if you're starting to read through, like the screen reader is reading through this,
[52:44] if the label's not linked to the input, it might say something like text box,
[52:49] I don't even know what it would say. I think it would just say text box empty,
[52:53] empty string or something. I'm not sure Ben can maybe let me know that.
[52:57] I'm not an accessibility expert, but basically it's super important
[53:00] to have these things tied together. And this is also important why,
[53:03] can that, can we hear that? - Nope, it just read everything,
[53:09] but at least this one version of it. - Okay, so yeah, so it's super important.
[53:16] So, and like, we can even test this. So, and this is another thing I'll show you
[53:20] in the DevTools. So, if you go in the DevTools at the top right there
[53:24] for the label element, double click on the,
[53:28] where it says for equals quotations in the label element, and just double click on the number in there,
[53:36] the 913EC whatever. - This one?
[53:40] - Yeah, just delete that. So, double click it and you can delete it.
[53:44] So, this is, there's two things here I'm gonna show. One, you can edit the markup or attributes.
[53:50] So, you can just like literally select it, delete it, and then click outside of the element and it's gone now.
[53:56] Now, let's click on the name input again, like let's inspect it.
[54:01] And you see, all of a sudden there's no more, you see it says generic, there's no label name.
[54:08] It's not connected to it anymore. So, if a screen reader was coming through here,
[54:11] it's gonna have no idea what it is. The text box says Gen Juno 'cause of the placeholder text,
[54:18] but basically a screen reader at this point has no idea what this field really is
[54:23] or like it can't communicate to the person. So, I just wanted to show the disconnect there,
[54:30] but also that you can actually edit the markup here. You can also change the whole thing.
[54:35] So, if you right click on that form, for example, in the panels on the right,
[54:40] just the form element up top there in the top part of the panel under the elements tab.
[54:48] - Elements form, yes. - Yeah, so right click.
[54:52] - Bye, Brittany. - Oh, hey, Caitlin.
[54:56] Caitlin's in my virtual coffee community as well as Collab Lab, which is a place we volunteer at.
[55:03] So, okay, so we can right click here and we can say edit HTML or edit as HTML, sorry.
[55:11] And you can literally change this to whatever. So, like do a command A to delete it all.
[55:19] And then just, I don't know, put like a paragraph or just say hello or something.
[55:25] - Can I do an H1 always because I forget what paragraphs are. - Yeah, so there you go.
[55:37] Hello, beautiful humans or human. And then if you click outside of that,
[55:40] you're gonna see your page changes. - That was fun.
[55:44] - Yep. So, some of this stuff might not always be useful
[55:48] because like if you're developing a site, like you're gonna have fast reloading and stuff and so on.
[55:55] So, like some of this stuff might not be super useful, but this is stuff you can do on live sites
[55:59] that you might not have access to. If you're just trying out things
[56:03] like what is the label look like if I put like a label that's 200 characters long
[56:10] or something, so you can kind of go in this. And another thing that we can do here now is
[56:16] if we go to the sources tab, which is the third tab, and you click on the two little arrows there beside page,
[56:27] and there's something called overrides. So, let's go there and then just say,
[56:33] click on the select a folder for overrides. And for now, like in your downloads folder,
[56:40] just create a new folder, I don't know, call it whatever, potato, stream, I don't know, avocado, whatever.
[56:47] - Potato, it's gonna be called potato. - My friend I use here as well.
[56:55] Okay, cool. So, now we have this folder now.
[56:57] So, now let's do something like, let's inspect TeachGen tech there,
[57:04] the word over on the left on your form, and let's inspect it.
[57:10] And let's go to the CSS, the styles tab, the one in the middle there on the left.
[57:17] - Why am I being super blind? - No, no, it's all good, to the left of that.
[57:24] So, the- - Styles. - Yeah, there we go. - And then the CLS.
[57:30] - Yeah, so let's add style to it in the element.style there. Let's just change the, just below it,
[57:36] where it says element.style, click in there, and let's just do color.
[57:41] Since it's black, we'll make it accessible. So, let's just put it back to yellow again or something.
[57:49] Press enter. Okay, it's set.
[57:51] Now, go ahead and refresh the page. Unless I'm talking out of my butt, it should keep it.
[58:00] Oh, why didn't it keep it? There's somewhere, what is it?
[58:05] The overrides allow you to save the changes, and I'm wondering why it didn't do it.
[58:10] Let's try that again. Let's go to sources again.
[58:17] - I was just wondering if it, like if you click that button, if it would,
[58:21] if it would play nice, but no. - Okay, so let's try it again.
[58:25] - Sources. - Oh, I think, okay, and if you open that,
[58:29] it should be empty, I think, that folder. - Yeah.
[58:33] - All right, let's go back to the elements tab again, up top there.
[58:38] Let's go to style again, and let's add that yellow again. I just say, sorry, color yellow,
[58:47] and then I think we need to save it. So, just do command S.
[58:51] I believe that'll do it. Okay, now let's go back to,
[58:55] oh, sorry, we gotta highlight the teach gen tech, sorry. I think we were on the wrong one there.
[59:02] Yeah, there. - Is it?
[59:05] - We can do the whole thing, if not, you could, but just the teach gen tech, if you want.
[59:12] And then let's go to the element.style again below there, and let's just do color yellow.
[59:16] And we're gonna just click command S after we've added that.
[59:25] I believe that'll do it. Now let's go to the sources panel up top there again.
[59:32] Let's go to potato and it, does it not have it? Weird, why doesn't it have it?
[59:38] Okay, try, why is it not finding it? - Oh, I don't know, I clicked something.
[59:45] - Oh, that's Grammarly. You can also, we haven't even looked at debugging yet,
[59:49] but you can actually debug and see source code of browser extensions too.
[59:53] Try refreshing the page. If it's not keeping it,
[59:57] I'm gonna drop a link to overrides 'cause I'm clearly forgetting something.
[60:01] But the main point of this is like, you can alter the page and like refresh it
[60:09] and it keeps your changes. It's not permanent,
[60:11] it's just like in this kind of override state. And you could look at that after if you wanted to,
[60:15] if you needed to pull some stuff out. - And bye, Ben.
[60:20] - Yeah, later, Ben. - Interesting.
[60:28] Maybe I forgot something. Yeah, specify directory.
[60:34] I'm not sure. - We don't need to dwell on it too much.
[60:44] Definitely take a read up on that again. I was doing it yesterday 'cause I was just,
[60:48] I was writing a list of stuff to go through for the stream and I was like, why is that not working now?
[60:54] But anyways, the main point is you can alter the site and you have it all saved in this like local overrides folder
[61:02] and this can be useful. I was actually changing the Netlify site yesterday
[61:08] with this. So like when you go to netlify.com on my own computer,
[61:11] it was saying like, what's up, Nick, you know, like- - Oh, that's so fun.
[61:16] Okay. - There's obviously great tooling for frameworks there too.
[61:23] So like some of this stuff might not be as pertinent, but okay, cool.
[61:28] So we've looked at that. We're going to kind of start looking
[61:32] at some JavaScript stuff now. So let's go back to the elements panel.
[61:37] And if you press the escape key, it's going to open up the console below
[61:44] and you can drag that up a little bit. And you can drag those errors
[61:50] that aren't necessarily from your site. You can see errors there from like browser extensions
[61:56] and stuff, but let's clear that. So if you just click on like the little Ghostbusters sign
[62:01] there, minus the ghost, and let's just drag the console down just a little bit.
[62:07] Okay, and let's drag the top part down a bit. I don't know if it's going to keep both of it.
[62:15] Okay, so let's click on body there in the HTML up top. - Top, top, top, top.
[62:24] - Okay, cool. So we've clicked on it.
[62:26] Now you're going to see, if you look to the right of it, it says equals equals $0.
[62:30] Okay, so now if you come into your console down below, type in $0 and press enter.
[62:37] Just, yeah, the bottom. - Oh, $0, enter.
[62:43] - Okay, yeah, so now you press enter. It's a reference to that element
[62:50] in the document object model, typically called the DOM. So you could do something like now you could do,
[62:58] you could actually modify stuff about this element in the console.
[63:03] So you could say, for example, $0, if you type in the console there for a sec,
[63:11] you could do $0.classname, which is a reference to the class attribute.
[63:18] And you get autocomplete here too. And then just say equals, I don't know,
[63:24] like red or something. Yeah, you can just, if you press the up arrow
[63:27] and then equals red, which won't exist, I'm assuming. Oh, you'll have to put it.
[63:33] It's a text, so you'll have to put that in quotes, but. - Oh, equals.
[63:36] - So just equals quotes red or whatever. And it should change.
[63:43] Yeah, you see how the body's changed all of a sudden? - Oh yeah. - Now, 'cause, well,
[63:48] one, class name red doesn't exist probably, so it's just, this is whatever it is without dark mode.
[63:53] There's a lot of things you can do here, 'cause you can obviously change classes and stuff
[63:58] in the CSS portion of the DevTools, but you could do stuff like you could add a click
[64:03] to the body as well. And for some reason, the debugger's on, I'm not sure why,
[64:11] but if you click the plus, the play button up top there in the browser, it's going to finish it.
[64:19] There's something, I'm not sure what's connecting to it. Just click play again.
[64:24] I wonder what it is. Weird.
[64:30] There's, I wonder if there's, I wonder if there's something in the site
[64:34] that's trying to debug, that's really weird. Okay, let's just refresh it.
[64:39] I don't know why the debugger keeps going, but basically what I wanted to mention about the $0
[64:46] is if you keep selecting other elements, you'll have like $0, which is the most recent one,
[64:53] $1 becomes the previous one. And you can basically have references to all these things
[64:59] and you can do stuff with them. You know, how valuable that is to you varies,
[65:03] but there's other things you can do in here. So you can do like, because it's the console,
[65:09] you can do stuff like in type console.log, hello or whatever, you know,
[65:14] which is not really that useful, but you can use this to also just check the state
[65:20] of certain things. And I'm still perplexed why your site keeps going
[65:25] into a debug mode for some reason, 'cause-- - Did I click something?
[65:29] I mean, knowing me, I could have clicked something. - It's possible, but it looks like there's something
[65:34] in the code that, weird. - That one was for Notion forms.
[65:41] So I don't know if-- - Okay, maybe there's something there.
[65:44] We can go ahead and close the browser tools, but, okay, cool.
[65:50] - Like all of these? - Yeah, and then we can just reopen it.
[65:53] We can go back to my site or to like dev two or wherever you had.
[65:57] - Let's go to Ben. - Okay, yeah, let's go to Ben.
[66:00] So let's go back. - Let's celebrate Ben's site.
[66:02] - Yeah. This is now an official Ben Myers appreciation stream.
[66:09] - Yeah, and they're no longer here, so won't even know about it.
[66:14] - Yeah, all right. So we can inspect in there again, literally anything.
[66:19] All right. So yeah, so now if you click dollars,
[66:27] type in dollar zero on the console again, you're going to get a reference to it.
[66:34] Okay, so now let's just do something. Some of these things aren't necessarily useful,
[66:39] like the exact thing I'm showing you here, but it's just to show you that you can modify the JavaScript,
[66:44] you can interact with it. So we can do dollar zero dot add event listener.
[66:50] And if you're used to frameworks, if you have like in React on click, this is under the hood,
[66:58] this is really what it's doing. So we're going to say add event listener,
[67:02] and then we're going to just click the up arrow. It's a native function.
[67:06] So we're going to do parentheses, and then we're going to do quotes, click,
[67:11] type the word click, sorry, and then close the quotes and then comma.
[67:17] And then we're just going to put a function. So we can do like a open close parentheses,
[67:24] and then do equals and then a greater than symbol. And sorry, yeah, the other way.
[67:35] - The other way? You probably said it, right?
[67:37] Doesn't mean. (both laughing)
[67:38] - And then let's just do something silly. Like let's just say alert, hello, beautiful human.
[67:43] - And then it would be in. - Oh, it's a function.
[67:51] So you'll put it in parentheses, sorry. (sighing)
[67:57] - Or we can put potato or whatever. - I always put hello, beautiful human,
[68:05] but you might see me putting potato more often now 'cause I grew up in Idaho.
[68:10] - Oh, okay, okay. - So the land of potato.
[68:13] - I always use potato for some reason. And then let's close the parentheses one more time.
[68:17] Let's press enter. Okay, so now it's going to return,
[68:22] it console logs undefined, and that's because typing out that code returns nothing.
[68:28] But click on the header now, the Howdy I'm Ben. Sorry, on the actual website.
[68:35] - Okay, oh. - So you can start doing stuff like that.
[68:41] And this can be interesting if you want to just test stuff or like so on.
[68:45] So that's one thing. We haven't even looked at the debugger really yet,
[68:51] but let's open up. - I mean, we only have 20 more minutes.
[68:56] So I'm down if you're like, this is a good breaking point. I'm down to have you on the show again.
[69:03] I think that a lot of this is also just sharing knowledge. And we got to do that a lot with like everybody
[69:11] on the stream earlier and using best practices. So I'm down for whatever you're up to.
[69:18] You're the one who knows all the knowledge. - Well, I'll definitely say I don't know everything.
[69:23] And anybody that tells you they know everything is they definitely don't.
[69:27] - Yeah, I'm like, I'm full time, it's full. - Yeah, yeah.
[69:30] Okay, so let's look at the debugger. So let's actually create a webpage.
[69:39] So let's go back. Let's open up VS Code.
[69:42] And like you said your current site's using Squarespace. Is that right?
[69:48] - Yeah. - Okay, yeah, so we won't use that
[69:50] 'cause we just kind of want to build something out here. We can even...
[69:57] Okay, so yeah, so you did the edge function with Jason last time.
[70:01] We won't necessarily debug that, but what we can do is let's go to your index.html file there.
[70:11] If we have time, we could debug that, but I don't think we'll have time.
[70:14] So in a webpage, you can actually have a style tag in there. You can also have a script tag.
[70:22] The script tag allows you to write JavaScript. The style tag allows you to add CSS.
[70:28] A lot of times you'll see in frameworks and stuff, they pull these things out.
[70:31] Like the scripts are all separate. There's a bunch of them.
[70:34] But for the purpose of just showing how the debugger works, we're just going to add a script tag.
[70:38] So right under line 13, let's add a script tag. So just literally just S-C-R-I-P-T for the script tag.
[70:48] Yeah, sorry, with the... - Right.
[70:52] - Yeah, exactly, yeah. - I'm like, why can I not talk today?
[70:58] Script, there we go, script tag. - Okay, cool.
[71:03] All right, so you already have this site running. I think you ran it locally with Jason last time.
[71:11] Okay, so in the script, let's just add something like, let's press enter.
[71:17] So we just have a bit more room here. And let's just type console.log, you know,
[71:23] let's go with potato 'cause I like that word and you're from Idaho, so.
[71:28] Okay, cool, let's save that. Now let's open up your integrated terminal
[71:34] or whatever you used for your terminal. And we can just run ntl dev.
[71:40] Just, yeah, just make sure you're in that folder of that project, wherever that is.
[71:46] Thanks for the kind words, IU, but I definitely don't know everything.
[71:52] - Make this giant, let's see. - Cool, cool.
[72:00] I can't remember, are you on East Coast as well or? - No, I'm on Mountain, I'm in Denver.
[72:07] - Oh, okay, okay. - Yeah, so, and then what is it to run again?
[72:14] - Oh yeah, so you can do, you can type in netlify or most of us at work, we use ntl,
[72:20] which is the short format. And then space, and then you just type dev.
[72:25] So this will run the netlify CLI in development mode. And the stuff I'm about to show you
[72:32] has nothing to do with the netlify CLI, it's just you already have a netlify project set up,
[72:36] that's the only reason why I'm saying use it. Okay, so let's open up the dev tools again.
[72:42] - Oh, let me close this other one, just so that way I don't get them mixed up.
[72:47] - Cool, cool. Okay, so let's inspect and let's go to this.
[72:56] Let's look in the, if we refresh the page, we should see our console log.
[73:05] If you, did we save it? - I thought I did.
[73:09] - Oh, you have that, you're, no, it's your detector thing's still debugging
[73:12] for some reason. You mind closing that file?
[73:15] I don't even know what that is. And it's so weird that it keeps going.
[73:21] Yeah, you'll have to click play in there on the blue plate. What?
[73:28] I have no idea what that is. (sighs)
[73:32] If you click on it, okay, it stopped. Okay, so let's just look in the,
[73:42] that was actually showing you the debugger in action 'cause it actually stopped,
[73:45] but I have no idea what that is. But let's, okay, yeah, there's something,
[73:50] I don't know what the-- - It's a DOM.
[73:52] I will tell you my extensions like to break things. So let me see if I can get--
[74:00] - Okay, you know what, let's do this. Don't remove anything.
[74:03] Let's do Command + Shift + N. It's going to open up an incognito window
[74:07] 'cause I don't want to mess up your setup or anything. - Why, what are you doing, computer?
[74:14] - Is that an incognito? 'Cause it's usually a different color.
[74:19] - Yeah, I'll just-- - Or worst case, just click in the Chrome menu up there.
[74:25] - Yeah, I was like, I'm just going to go this way. I don't know what it's doing.
[74:27] - Okay, okay, so there's no extensions here now. - Okay. - There we go.
[74:35] - Cool, all right, and let's open, yeah, we can close that.
[74:37] And let's just open up the DevTools for here. And a side note, but if you're--
[74:43] - I hit View Page Source instead of Inspect. - Oh, okay.
[74:47] All right, so, okay, already this is working better. A side note, if you ever run Lighthouse,
[74:53] 'cause there's a Lighthouse tab in the DevTools, and this will give you a score,
[74:58] like performance, accessibility, and all that, always do it in an incognito window
[75:02] because you won't have your browser extensions there 'cause they can actually affect the Lighthouse score.
[75:08] - Oh, okay. - So that's just a side note. But, okay, so let's look in the DevTools here now.
[75:12] We're going to see that it console log potato. Okay, so we're in good spot here.
[75:18] Okay, so now let's go up into the sources there. And let's go to page,
[75:27] the one just to the left of overrides. And let's click on the index there.
[75:32] Okay, so this is our actual page that got rendered. Normally you would have JavaScript files too,
[75:38] but I'm trying to keep it simple for now. So if you click on the number,
[75:42] just to the left of the number 15, it's going to add a little red dot,
[75:47] like literally in the gutter there where the number 15 is. - Oh, yeah.
[75:52] - Okay, so it's going to add this. It looks like a little kind of bookmark.
[75:55] This is called a breakpoint. So now let's refresh the page.
[76:00] - Let me move it. - So you can do a command R or just however you want to do it.
[76:08] Okay, so you can see here, it's actually stopped the program.
[76:14] You see how it says pause in debugger. And then now if you click play,
[76:18] so it's literally paused your program, whatever's going on.
[76:22] And then now it's going to run and it says potato. There's not that much stuff useful with the console log,
[76:27] but that's just the starting point. So now let's go back to our webpage in the VS code.
[76:34] Cool, and let's add something else in here. Like let's add a function.
[76:42] So in the script tag area, we can still leave the console log, it's okay.
[76:47] Let's create a function. So just literally the word function and then space
[76:52] and let's, I don't know, like, hello. And then we'll open parentheses and we'll give it a,
[76:59] it'll take a parameter. So something that it can accept as input.
[77:07] So let's just say text. So this, and then, sorry, it's going to be,
[77:14] just the app, it's a variable name here. So our, not variable, parameter, sorry.
[77:20] Okay, and then let's open up squiggly brackets. Don't worry about the formatting it,
[77:26] like prettier is not happening or anything, it's okay. And let's just type, we can do a document.body.innerHTML.
[77:34] I'll explain what this is if you're not familiar. And then we're going to say plus equals.
[77:47] And let's put quotes now, 'cause we're going to be adding text here.
[77:53] Or yeah, and then let's just say, hello. And then after, or we won't even use potato.
[78:03] Let's just say hello with a space. We can use something else called a template string,
[78:08] but I won't bother with that for now. So after the hello, just put a little space
[78:12] before the quote, and then after the quote, let's add a plus, and then we're going to say text.
[78:18] I guess we could have called text name, but let's just go with that.
[78:24] Okay, so what this function does is it finds the body element on the page,
[78:31] and the innerHTML is literally all the HTML within the body tag, and it's going to,
[78:37] the plus equal means it's going to add to the end of it the words hello plus whatever the text is.
[78:43] So that's the function we're going to have. And then after line 18, let's press enter.
[78:48] And just to make this a little more interactive, we're going to do something like document.body,
[78:59] and we're going to do addEventListener again, like we did before.
[79:04] And you should get some IntelliSense here 'cause you're in VS Code.
[79:08] So, sorry, dot addEventListener. And then we're going to do the same thing,
[79:16] so parentheses, and we're going to do quotes click. And then we're going to add a function after.
[79:26] So we're going to, sorry, not function the word, still in the addEventListener.
[79:35] After the click quote, we're going to put comma. And then we're going to say,
[79:41] let's do open parentheses, close parentheses, and then equals, and then the greater than.
[79:47] And then let's just say hello, which is our function we created up there.
[79:55] And let's just say gen or something in parentheses, and it has to be in quotes 'cause it's text we're adding.
[80:02] So at this point, we're going to be calling the function. Okay, so let's save that.
[80:08] And now let's go back to the browser. And let's go to the browser dev tools.
[80:18] We should still have that open too. - Yeah, I need a refresh, right?
[80:22] Let me save this. - Yeah, let's give a refresh. - Refresh.
[80:29] - Okay, so let's remove that breakpoint there. So if you click on the, yeah, exactly.
[80:34] But let's add one on line four. So if you go down below there in the JavaScript,
[80:40] just click on, or sorry, line 17. Okay, so now, so just looking at the code just to explain,
[80:48] if we click on the body of, so basically anywhere on the page,
[80:53] and a click happens, it's going to call hello gen. So let's click on the page.
[80:58] Okay, so now you're going to see what's happened here is the click did actually happen,
[81:04] but now we're using our debugging tools. So this is the JavaScript debugger
[81:08] that we're looking at right now. And you can see right up top there,
[81:13] I don't think you can zoom it in 'cause it's part of the browser,
[81:15] but it says paused in debugger. And now if you click the play button, go ahead,
[81:21] you're going to see it adds hello gen to the rest of the page.
[81:24] This is a trivial example, but let's click again. It's going to stop here again.
[81:31] Now let's make the browser dev tools a little bigger. Like we can hide the webpage for a second here.
[81:35] Like we can give the full screen to the browser dev tools. And I know we're close to time here,
[81:41] so we'll just kind of touch on this today and definitely happy to come back on again if you want to.
[81:46] So there's a lot of things that we have available to us here. So first thing is if you hover over things
[81:54] like in the middle panel there, you get information about it.
[81:58] So like when you hover over document, that's the whole document,
[82:01] which is literally the entire webpage and you have information about it there
[82:05] that you can look through. Same thing if you hover on the,
[82:09] if hovering over body won't, because it's document.body, that's the whole thing.
[82:13] - Oh, okay. - But there's some interesting things
[82:17] you can see here already. So like on line 16, where it says function hello text,
[82:22] you can see that the value that you put in in the click there, gen,
[82:25] it's showing up to the right there. It says text equals gen.
[82:29] And so like all of a sudden you're getting all this information that's helpful to you
[82:34] in the context of like, say you have a bug, like, oh, why is it always, you know,
[82:38] when I click, why does it always say gen? It should be saying Nick in some cases, you know?
[82:42] And like, again, this is a trivial example, but you're like, oh, well, it's 'cause I set it to gen.
[82:48] That's why it's not working. Okay, problem solved, sure.
[82:50] But there's other information you can see here. So the first thing is break points.
[82:55] So it's telling you all the places where you have break points,
[82:58] 'cause you can have multiple of them. Like if you click on the console a lot, exactly,
[83:01] you can click in a few places. The other things that are interesting
[83:06] is if we close the console for a second, on the bottom right there, just click on the X,
[83:11] just so we have a bit more room, you're gonna see there's a bit more information
[83:16] to you on the right there. So there's a scope section,
[83:19] and you can see it says local, and like this window and so on, and text gen.
[83:25] So basically, it's giving you all the information. This, in this point here, means the entire browser window.
[83:32] There's a whole thing if you wanna read up on JavaScript in this keyword.
[83:37] - Okay. - And I can link to some of that stuff.
[83:41] But basically, you're getting all the information about the current context you're in.
[83:45] Like I clicked on this thing, I can see that text is gen, and then there's some global information too,
[83:53] which is related to the whole thing. So like, for example, on global, there's the alert function.
[83:58] So like alert, like if you say alert hello or something, and so on.
[84:02] We don't have anything too complex here right now, so there's not a lot of information there,
[84:07] but this can be helpful. The other thing is there's this watch panel up top there,
[84:12] just under the paused on breakpoint. Let's open that,
[84:16] and let's just click on the plus sign on the right there, and let's just add, type in the word text and press Enter.
[84:24] And all of a sudden, you're going to be like, okay, I can save some things on the right here, you know?
[84:29] I could add other things. So like, you know, maybe you want to test something.
[84:32] So if you click on the plus again, you can say text, text plus, you know.
[84:37] Oh yes, no worries. You can say text plus, you know,
[84:43] hello or something in quotes. Again, these are trivial examples,
[84:48] but it basically, you can start having some stuff like, hey, I want to see some things here,
[84:53] just have them on my sidebar so I can see, because what could happen is say like,
[84:57] maybe you happen to be looping through something and like text changes all the time.
[85:01] So like, what does it look like when text plus this other thing happens and so on?
[85:06] And basically, there's a bunch of stuff you can put in there.
[85:09] There's some more stuff in here that's potentially advanced for a beginner potentially,
[85:17] but there's this thing called the call stack, which is something good to learn about,
[85:20] but it's literally like, you can see there's a blue arrow right now
[85:25] and it's pointing to the hello, and that's because we're in the function hello.
[85:29] And then before that, it says there was anonymous and the anonymous is actually the function
[85:36] where we're calling hello. If you click on it and it shows you where it is.
[85:39] And this can be helpful if you're like, you know, where is it?
[85:43] Like, how did I end up at this function? And the call stack can actually show you
[85:47] where it came from, like where it originated. Basically like think Hansel and Gretel,
[85:51] follow the cookie trail back to like... So, and there's a lot more things you can do in here,
[85:58] but I know we're close to time and I actually do have a hard stop at 1.30
[86:03] 'cause I forgot I have a one-on-one at 1.30. But this is, like I said,
[86:09] it was kind of like a whirlwind tour of the developer tools in the browser.
[86:13] And all these things I showed you here today, they all exist in Firefox.
[86:18] In Safari, they have similar stuff, but they're not as far ahead as Chrome
[86:26] and Firefox in terms of dev tools still. They're getting a lot better,
[86:31] but I just thought this would just be interesting to just kind of give,
[86:35] it's not too shallow a dive into things, but 'cause there's honestly so much stuff in here
[86:41] and like we could dive on one particular thing and probably spend at least an hour, you know?
[86:46] So it's really just kind of to give like, here's an overview of like a lot of things
[86:52] you could use in the dev tool. So hopefully folks have found that helpful.
[86:56] - I will say, yeah, like it's definitely helpful and something that I think would assist going forward.
[87:05] And also like seeing that you were on like Anthony's channel and like you went into much more detail on those.
[87:12] It's like, it's such a wide topic. That's why Ben's been on the show so much, so.
[87:17] - Yeah. Yeah, I guess the last thing I'll say about it is like,
[87:23] for folks that have been doing, who might be new to Node.js or even something like Dino,
[87:29] which is from the creator of Node.js, we use this at Netlify for our edge functions.
[87:34] I don't know, I think Jason mentioned that on your stream, but you can actually use the browser tools,
[87:42] like how we were debugging there. You can actually debug backend JavaScript code
[87:46] in the browser as well, using literally the same tools. And the other thing we definitely didn't have time
[87:53] to look into is in VS code, all those tools for debugging, we can actually do those in VS code as well,
[87:59] which is another thing we could look at another time if you wanted to, or we can honestly even talk about
[88:06] something completely different, automation, OBS, who knows. - I feel like automation would be such a cool one
[88:12] to talk about, but y'all, I know that Nick has a hard stop, so I'm going to start the raid really quick,
[88:18] just so that we, yes, VS code debugging. Nick is just going to, you know, come on the stream.
[88:26] He didn't know that you were going to get, you know, volunteered to go.
[88:30] But all right, y'all, I am raiding you now, and thank you everyone that has showed up today.
[88:38] Let us know questions, and let me hit end. And, yeah.

