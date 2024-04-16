---
showLink: "https://www.youtube.com/watch?v=HilfyKUdsT0"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-web-layout-patterns-with-travis-waithmair"
title: "Teach Jenn Web Layout Patterns with Travis WaithMair"
publishDate: "2022-08-08"
coverImage: "https://i.ytimg.com/vi/HilfyKUdsT0/maxresdefault.jpg"
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

[00:00] Hello, beautiful humans, and thank you once again for joining Teach Gen Tech. Today we have Travis with us, and Travis, please introduce yourself and what you're going to teach us.
[00:11] Yep, I'm Travis Waithmer, and I'm famous for having, or infamous, whichever you would like to think of, for having a layout library called Bedrock Layout Primitives, and I also am a
[00:27] software engineer at Plex. And, yeah, today we're going to be going over just web layout patterns and different, like, ways to lay out the web. And, like, I get the words you're saying.
[00:41] I do, I do. I, like, the words you're saying do make sense, but when we're saying the way you lay out the web, is that, like, the way a website just shows up, like, the front end of or style of
[00:58] a website? Exactly, and every, and it's not wrong to group everything as just one big style because we use CSS for it, but I really think it's, like, web layout as, like, a separate concern than,
[01:13] than, like, the prettiness of it. So, like, the colors and all that, that all uses CSS, and that's great, but also the layout is a totally, kind of, like, sub concern in my mind,
[01:26] and that's how I like to think of it. So, I think I like to separate that, kind of, both in the code as well as, like, how I approach the web page and how I structure it,
[01:39] because the way you lay out the web page is, it creates, like, a hierarchy and different things like that. So, as you read, like, you're, like, it points your eyes in different places.
[01:52] So, knowing how to do that layout is really important, and it gets really easy to, like, kind of, associate, like, everything is just style, but, like, I really like to just pull
[02:03] it as, like, separate things, in my mind, at least. >> I'm digging it. I'm digging it, and that is making sense, but I like the way you said making it pretty, because that is when I think of,
[02:16] you know, web layout. In my mind, I'm, like, how you make something look pretty, not necessarily functional, but is there, like, a certain, like, go-to web layouts, like,
[02:31] or I'm not sure how to say that one correctly. >> So, there are some, like, and that's where I want to get to, like, this is where a lot, and most of, I should say most of my career,
[02:41] a lot of my career, I associate that everything is the same, and I do, like, a lot of people do when they write CSS, is you just throw mud on the wall, and then it works, and then it's,
[02:51] like, don't touch it. Like, it works now, so don't change my code. It works, but, like, there's some actual, like, if you just, like, anything, there's, like, patterns that we follow,
[03:01] like, if you go to web pages, they're not, like, 90% of the time they're doing the same things. They're just doing, they're just combining these patterns in different ways to achieve these
[03:14] things, but if you break it down, they're following, like, probably, like, a handful of, like, layout patterns, and so if you just, like, create those patterns and learn how to do those,
[03:23] you can get, like, most of the layouts on the web. It's kind of, like, when learning a language, there's, like, 1,000 words, and most, like, somewhere around 1,000 words in most languages
[03:34] gets you, like, 80% of the way there. It's just kind of the same concept, like, just a handful of, like, web layout patterns when composed together will actually get you most of the things you need
[03:46] done, and so, hence, that's what I do with my library, but even if you don't use my library, that's, if you think about it that way, think about, like, what pattern we're doing,
[03:57] you can do, you can get really far in web layout world. Okay. Okay. Like, it's starting to sink in, and I'm totally going to sidetrack myself to go,
[04:11] because I believe it's on, linked on your Twitter, right, with Bedrock? Yes. Because I feel like I should definitely show people that, too.
[04:24] So, there's a library, yeah, bedrock-layout.dev, and there's a React component library, as well as a CSS library version of it. Okay, yeah, let me pull it.
[04:41] Here we go. Let me make this a lot bigger, because this is the part about streaming that I always forget, is to make things bigger. I do the same thing all the time. Anthony,
[04:53] who's been on your stream before, is always like, Travis, bump up your, your. I know, right? He's going to be on later this week, and because he's tired of me not looking
[05:05] at the readme, or, like, creating good documentation, he's like, Jen, you need to start doing, okay, okay. He always reminds me of, like, the big brother that is always mad at you,
[05:16] because you're not doing it, and, like, just cares, because he just really wants you to do a good job. That's what Anthony reminds me of. Exactly that. He's a great guy.
[05:25] Okay, so, we have the layout here, and I love how you just have this as a resource that people can use, and I'll definitely have this linked afterwards, and I will link it in the chat
[05:41] really quick, so that way, everyone can take a look, too, and then, all right, so, just to show them this resource, we got that done. Now, what are we doing today? Oh, I thought we would do
[06:01] the fun thing that probably everybody has to do in a web page, is create a landing page, and I've already got a starter for you, and we're going to actually just focus on doing layout.
[06:14] Okay, I'm going to see if I can make this a bit bigger, so, there we go. All right, so, we got your database starter. I like it. Yes.
[06:26] Yay, I'm following you now. Sweet. I'm more popular already. Yes. So, yeah, so, if you go down below, you'll see we have a database, and we've got the, kind of,
[06:42] to show, like, what's actually there. Yeah, I was like, how do I scroll with the normal scroll and not even use it? You may want to do the, if you change the layout,
[06:53] instead of having everything on top, maybe put it on the side, so, if you click that, there's that button up at the very top, next to settings, it's got, like, the three squares and
[07:03] the big one, and there we go. Oh, I like that. Thank you. So, we got our, now I can make it bigger again, our database. I like this. I just like the name. Awesome. Now, the,
[07:18] you can see, like, everything's, like, looks pretty, but it's not laid out pretty, and so, that's what we're going to be doing today, is just focus on getting this
[07:29] laid out in a, in a nice way. All right. So, the first pattern, the first, like, thing that I thought we'd do is what I like to call the cover pattern. The idea is that it's
[07:44] going to cover an area and then center some children inside of it. So, vertically center it. So, I like to call that a cover pattern, and that's one of the nice ways of also thinking
[07:58] about these as patterns, is you can quickly just identify, hey, this is a cover pattern, or it's this pattern with this pattern, and it makes it a lot easier to think about what you're
[08:08] doing and how to approach it. So, yeah, let's go ahead and start this, and we're going to do this on the CSS. Okay. Can I close the HTML then, or are we? We're going to go back to the HTML. We
[08:23] don't need the JavaScript, but, like, yeah, let's just do CSS for now, and then we'll go back and forth. Okay. But if we scroll down all the way to the bottom CSS, we're going to start here,
[08:33] and we're going to use a different method of selecting than probably most people typically do. Usually you'll do, like, a dot, you know, class name of some sort, right? But we're going to use
[08:49] data attributes instead for selecting. Okay. And just because we're going to be creating these, like, these, like, utility components kind of thing, and I think it's helpful to kind of
[09:03] separate them out from, like, your regular classes, pretty, so it's easier to think of them as a separate concern, and this is a great way to do it so that you can also, like, not have
[09:14] to worry about these things, like, conflicting with your CSS later on down the road. So, to select for data attributes, instead of using dot a name, you're actually going to put it in square
[09:27] brackets. So, you do square bracket, and then do data dash, and we're going to do cover. So, this is a cover pattern. And then next to it, go out of the square bracket, and we'll do the
[09:40] curlies, and then we can write our CSS in here. >> Can the curlies be next to it? >> Yeah, that's exactly. Yeah. We'll just do that. So, inside the curlies, let me bring up my notes
[09:55] so I don't forget things. Okay. So, first thing we're going to do with this cover is we want everything inside of here to be in a column. So, we're going to do display flex.
[10:12] Actually, let's put this on a new line here. So, inside the curlies. Yeah, there we go. And we'll go display colon flex.
[10:29] And so, we're purposely giving, we're telling, whatever we're going to use, use the flex layout pattern display. And then, sorry. And then we're going to go flex direction column. So, do a
[10:42] semicolon after flex. And then, below that, we'll do flex dash direction colon column. >> Now I have to remember how to spell column. >> I always do, too. So, this will say, hey,
[11:08] everything's going to be, like, try to be in a row by default. But by changing the direction to column, now it's going to put everything stacked on top of each other.
[11:17] >> I'm trying to go away. You're not going to go away. Fine. I tried. >> So, we're going to do that. And then, the next thing, sorry.
[11:29] And then, the next thing we're going to do is we're going to do, let's just do a gap. So, that new line, and we'll go gap colon. And for now, just do one rem.
[11:45] We're going to come back to this in a moment. >> You said one rem? >> Yeah. One rem semicolon. >> I'm learning all the things today.
[11:57] >> And then, let's do a minimum block size. So, M-I-N, sorry. So, min block size. Min-block-size. And we're going to do 100 V-H. That stands for view heights.
[12:22] >> Okay. >> Semicolon. There we go. So, we're going to start with just this. This will be good. So, now, let's go back in the HTML.
[12:31] >> Does this one autosave? >> It should autosave by default. >> Okay, cool. >> So, let's go to the very top.
[12:42] And we're going to go on that header, right next to the header. So, we have header class header. But right next, inside the header HTML itself. So, yeah, before the class,
[12:57] we're going to just put data-cover. And then space. And you can see automatically that header section now is picking up 100 view heights.
[13:12] And there's at least >> I undid it so I can see it again. >> Yeah. There we go. So, that's cool. We're only part of the way there to, like, making this,
[13:34] like, really customizable. But, like, you can see already, like, we're covering a section. And so, the next thing we're going to do here is we want to make it so that sometimes we don't
[13:50] always want to cover 100% view heights. That's a good default. Because, like, say this is a hero that we're building up here with this header. Oftentimes we want to have it to be 100% view
[14:03] heights like this. >> I'm having fun with 100% view heights. So, that way because it shows, you know, like, this is the view height. So, it goes to it. This
[14:13] is really cool. But, you know, I can see what you mean by we may not want that. >> Yeah. I mean, sometimes you do, sometimes you don't, depending on what kind of thing you're
[14:24] doing. So, let's go and let's make this a little bit more customizable. And so, what we're going to do is we're going to instead of using 100% view height, let's go in let's go back down to the CSS
[14:39] and let's have this take a custom property. So, let's get rid of the 100% view height there. And let's do var and then the parentheses and do dash dash max and then with a capital W height.
[15:03] So, max height. And then let's do a comma after that. >> In the same bracket or a different bracket? >> Yeah. Right after the max height. So,
[15:16] yeah. And then let's do 100 VH. So, what this says is we're going to take the value of a custom property called max height. But if max height hasn't been defined, we're going to fall back
[15:33] to 100% VH. So, we have a default value that we're always going to use. But we're going to have a way for you to customize and change that. >> As a heads up, our number one fan
[15:45] who we were talking about earlier is here. Hello, Anthony. >> Anthony, welcome. We're building yeah, we're rebuilding Bedrock Layout from scratch.
[15:57] So, we're going to rebuild exactly what the library has already built. >> Yay. So much learning. >> So, this is yeah,
[16:12] I don't think I've ever really gotten into this level of detail with anybody on any other stream. So, you're special, Jen. >> Thank you. You both said so. I
[16:22] think it's definitely something it's a challenge to break stuff down this far. Because when we learn something, a lot of times we're like, oh, everybody knows that. But because we forget
[16:35] that we started there a long, long time ago. So, I do appreciate it. And I haven't done much in CSS. So, this is pretty exciting. >> That joke came in.
[16:46] >> What up, Akari? I hope you made it home safe. He had a layover in Denver yesterday. And I was like, dang it. I wish I knew. Because I live in Denver. So, but you know.
[17:00] >> I've been to Denver twice. And one of them was not a great experience. Because it was we picked up from let's find out of Salt Lake City. And as soon as we got in the air, they said,
[17:12] our AC's broken. Or our heater's broken. So, we need to land in Denver and fix the heater so we can fly. I was flying to New York. Because we can't wait this out. You guys will be freezing.
[17:26] But then they're like, we can't land in Denver. We have too much fuel. So, we flew above Denver for an hour. Just circled. And then landed. >> That happens. I've done that in Denver, too,
[17:37] where they just circle it. Because but it was normally that happens it's happened a few times because of the storms. I need to tell my dog that she is not part of the live stream today.
[17:50] >> Are you sure? She is now. >> Everybody might hear her whining in the background. But it's not me. It's the dog making very random noises. Okay.
[18:05] So, we changed it to max height and then 100 VH. >> So, now we can customize this. So, if we go back up to the HTML. And right in there, we're going to do an inline style. So, if we go
[18:20] style. >> Where should I do it? >> Sorry. Right after the word cover, do a space. And let's write style equals. And then do a string. So, sorry. Do a quotation.
[18:38] >> Is that right? >> Yeah. And then we'll go we're going to define this property here. So, we can go dash dash max with a yeah, exactly. And we'll go
[18:52] colon. And let's do 50 VH. Yeah. Lowercase VH. Yeah. >> I was like I typed that one wrong. So, we did width or we did height in CSS and we do width here.
[19:12] It should be VH for both. Oh, did I say max width? I meant max height. Sorry. My brain is just like... >> I already told you that, you know, with my cat bite yesterday, I'm off in La La Land half the
[19:31] time. At least talking to you beforehand, I caught that I don't have the rings of swelling on there now. All right. So, we got max height and I like how that changed it where it's not crazy and all
[19:47] over the place. >> Yeah. So, yeah. So, this will allow us to use that same cover component anywhere else if we need to. We want to follow this pattern. And we can customize that max height.
[20:00] Now, one might ask, like, why don't we just why max height or and in fact, we're using the wrong thing. I really should have said min height. Let's go back and fix that. See, I have this in both of
[20:15] these. Because, yeah, min. Because that's really what we're doing. We're saying the minimum height is 50 view heights. But the reason why we want to say minimum is if we actually had content in
[20:38] there that was higher than 50 VH, we want it to be at least the content height. We only want it to be a minimum 50 VH if we have less than 50 VH worth of content. So, that's why we do minimum height.
[20:51] So, we can say cover at least this amount. But if you have more content, definitely keep pushing, keep going. So. >> I dig it. >> So, most of the time, whenever if you with the web, you don't
[21:05] you hardly ever want to set a fixed height. You don't want to say, hey, the height is this. Even though practically it may only never be that. You want to do minimum height because it allows it to
[21:18] be resilient in case the content pushes it out. Some of the memes around CSS where things like overflow out of bounds or different things like that come from when we try to control the content
[21:32] and try to say this is like try to control the web like we do like a magazine or something like that. Where we know exactly what the content is going to be like in advance. But the thing is on the
[21:44] web, we don't know what it is. It could be like only a couple paragraphs or it could be like 100 paragraphs. So, we need to be resilient. And that's why using minimum height makes it resilient.
[21:55] >> You're piecing so many things together for me because I do use Squarespace for both the podcast and this live stream. And in Squarespace, it allows you to edit the header.
[22:09] And now that I'm like, I'm like, oh, so is this how you can make all these changes? This is cool. Please continue. >> Yeah, no problem. So,
[22:21] I talked about it already that like the other part of the web layout, the cover pattern is not just that it like covers a section, but it also centers vertically centers some children if you want it.
[22:31] So, we're going to implement that part now as well. So, let's go underneath inside the actually, we're going to do this on a separate line. We're going to create.
[22:44] So, go to a new line and we're going to do once again, data dash cover. So, we're saying, hey, anything that has a cover and then next to it,
[22:58] don't, we're not going to do that yet. So, we're going to do the great, no, sorry, less than I can, it's the arrow that points to your right. Yeah, that one, sorry.
[23:11] >> Okay. >> Is greater than yes, the greater than symbol. And then we're going to do square brackets again. And we're going to do
[23:21] data dash cover dash children. Yeah, do we want to do that? Yeah. Or no, let's do centered, the word centered. There we go. And then after that, we'll do the square, the, yeah, curly
[23:44] brackets. So, first of all, what is this selector we're doing? We're saying anything with a data cover that has a direct child that says data cover centered, we're going to add these styles.
[23:58] So, we could add data cover centered on anything out there and these styles won't apply. It's only going to apply if we use the data cover centered attribute on a direct child of the data
[24:12] covered element. >> Okay. >> So, that just so we're clear and we'll see that in practice. It'll make more sense as we use it.
[24:23] But that's what that arrow bracket is saying. We're looking for the direct child that meets this qualification. >> Okay.
[24:31] >> And in here, we're going to do margin dash block. And we're going to do auto. >> Is that how you spell margin? >> Yeah, that's perfect.
[24:46] >> Okay, cool. I was like, I don't think I actually know how to spell margin, but that's okay. >> So, what margin block means, most people probably have learned like margin top,
[25:00] margin bottom, margin left, margin right, or margin, yeah. And those were great, okay, the web. But as the web has developed, we found and really have acknowledged that there's
[25:12] more writing styles than just English left to right. They've gone back and they've revamped and they've created some more logical properties around that. So, they've now added things like
[25:26] margin block, which means things in the block direction. And block direction in the case of English left to right is from top to bottom. But block direction, if you're in a vertical language,
[25:41] is actually left to right. Unless you're vertical right to left, then it's right to left. >> Got it. >> We do this because, once again,
[25:52] it makes our web page more resilient, makes our elements more resilient to any language that we may adopt. Or if we're just playing around and goofing around and we want to do something cool
[26:04] and change the writing style just to make it look pretty, we're still resilient in that case. So, anyway, yeah. So, margin block basically means the margin in the two block directions. So,
[26:19] the top and the bottom. Since we're in English left to right here, that's the top to bottom. And bottom. We're getting basically two properties as being assigned for one.
[26:30] So, it was really nice and easy. That's the other advantage with these new additions to the CSS. These are CSS logical properties. >> Got it.
[26:39] >> So, what we're going to do, we're going to go back in the HTML. And in there, right now, we have this below the figure, we have this H1
[26:53] that says database and the paragraph. So, let's wrap both of those in a div. >> Right? >> Yep. And then we'll put
[27:07] the ending tag after the paragraph. Perfect. And then... >> It's like changing things. This is fun. >> It's interesting that it's formatted that
[27:22] way. But, anyway, yeah. So, inside the div, the opening tag of that div, let's do that data covered. You're doing that inside the HTML itself. >> Oh.
[27:34] >> So, go all the way to the div and we're going to add this. There. Yeah. >> Here? >> Perfect.
[27:44] >> Okay. >> Go data, cover, and what do we call that? Centered? >> Yeah.
[27:52] >> Yeah. >> I think center. I'm going to look. >> Is it center or centered? Yeah. >> Centered.
[27:59] >> Okay. And then you probably can't see it on here because we're probably taking up the entire content. But if you were, like, to change the size for the main page there,
[28:17] maybe scroll up and see. Let's maybe... Yeah. You can see a slight change. Let's, like, maybe bump it. Like, really exaggerate it. Like,
[28:40] really bump up the size. Make it really small. Just to really show. So, yeah. You see, like, that database is, like, vertically centered right there inside
[28:53] this section. So, that way, yeah. Now we can do that thing where, like, you have that hero and then you, like, have that vertically centered, like, content right there in the middle.
[29:07] Sometimes you... Oh, anyway. So, yeah. This is... Yeah. That's all I want to talk about that. So, this is a covering pattern. So, if you're, like, hey, look, I need something to take
[29:19] up some content and vertically centered, this is the pattern you would want to use as a cover. Now, the other thing we want... Another good pattern that we use on the web all the time is
[29:29] horizontally centering things. So, we're going to do that one now. So, below the data cover... So, yeah. Below all this, let's create a new line. And in brackets, let's do data center.
[29:45] Would I do data cover again or just data? No. So, this new one is not related to cover at all. So, it's a new pattern all on its own that we're going to be... And let's just call it center
[29:57] itself. Perfect. And then let's do the curly brackets. Now, the center, the idea is we want whatever we have in there to be...
[30:12] To center itself inside of its content. But also to... Based off its content. But we also want to maybe have a fixed width. Like, a max width that it will grow. So, that way, like, it will be
[30:31] centered within... It will be, like, only a certain size and then center itself within that. And it will be more obvious once we do it. But that's the pattern that we're trying to do.
[30:41] - I'm just thinking... And this is me not knowing CSS as well. But would it be, like, display center and then, like, something along the min block size would do, like, min or max width or something?
[30:57] - Yeah. You're, like, on the right, like, idea here. So... - Okay.
[31:02] - Exactly. So, interesting. Like, there's so many ways to horizontally center things on the web. But one of the most, like, tried and true and still works, like,
[31:12] pretty much in every situation, every context, is to use the margin auto. Not in the block size, but in the inline. So, we're gonna do margin inline. Auto. Perfect. Now, the other thing
[31:33] about the center, though, is that it's also content. It's really based on the content. And so, I kind of, like, waved my hand on this. I brought in a reset, like, a CSS reset
[31:48] in here already that makes everything box sizing border box. Because that's more intuitive most of the time. But in this case, we're gonna re-put it back to the default. So,
[32:02] we're gonna do box sizing. Sorry. Let me make my notes here. Box sizing. And let's do content box. - Is that right? - Yes. Let's do a semicolon there,
[32:33] obviously. - Okay. Cool. - And then just for now, let's do, like, just to give it a value for now, let's do max
[32:41] inline size. So, max dash inline. - Dash size? Okay. - Max inline dash size. Perfect. And let's
[32:58] give it, like, 500 pixels just for the fun of it. Just for now. So, now let's go back up to the hero where we put that data covered centered. And let's add another
[33:19] attribute right next to it. So, let's do a space there and do data center. There you go. And you can see, like, because we put that max width there,
[33:33] that it's automatically, yeah, it's only gonna cover that 500 pixels. And it's gonna automatically, whatever margin is available, it's gonna put those in the inline direction on both sides.
[33:46] - Okay. And that's because in the HTML, we did it as the div on the H1. But would these still work if we added it to, like, a div down here?
[34:04] - Yeah. We could put it on anything in here. So, if we're, like, hey, that article or, yeah, anything on here, we could just put it on anything that we want
[34:14] to have to be, like, horizontally centered. And you don't necessarily need to wrap it. You just, if you have multiple things that you need to, like, have centered like that, you could wrap
[34:25] it. But if you're, like, hey, this article and just this article I want to be centered, you can go add that data attribute on that article.
[34:33] - So, I would just leave the article and then put it between article and class? - Correct.
[34:43] - Mind-blowing, right?
[34:49] - It is mind-blowing. It's fun seeing it, like, instantly, too. - Yeah. This is what I love about the frontend. There's just, you get such instant feedback
[35:03] for the things. - Yes. Instant gratification.
[35:07] - Yeah, exactly. Now, obviously, 500 pixels, that's not something that, like, is going to translate. We want to maybe follow, like, we need something to be more customizable.
[35:16] And so, let's do similar to what we did with the max height, we're going to do with max width. See, this is what the problem was. I had max width on my brain because I was already looking ahead.
[35:25] So, I screwed up what I was telling you to do. But, yeah, let's go. - Max width?
[35:32] - Yeah, max width. And then, let's do a comma. Let's do 100% just as a default. Because by default, we don't necessarily want it to, like,
[35:43] squish. Let's have it, like, just take up the entire width by default. - And that should automatically update because we already have that in the HTML.
[36:00] - So, in this case, we don't need to, like, do anything. For this, it's already, like, kind of covering that. So, now, we've achieved one of the most desired coveted things, which is
[36:14] a vertically centered content and a horizontally centered content. So, now, we've achieved nirvana on the web here. I'm just kidding.
[36:26] - We made it. Done. Easy peasy. We learned it all. - We're done. We're experts. No.
[36:33] - Just kidding. Just kidding. I know it is. There's so much more there. - Let's see. I want to make sure. Oh, yeah. So, the really cool thing is we can take this
[36:46] even one step further. We can actually, like, look for specific values. Because these data attributes, we can give them values, and we can do selections based off that. So,
[36:59] right below data center there. So, no. Actually, sorry. We're going to do a whole new, like, so, on a new set of selections. So, yeah. So, let's do the brackets, and we'll go data center again.
[37:20] Now, this time, though, we're going to do after the word center, we're going to do a tilde. So, it's the button right next to the one. But you have to hit the shift key.
[37:32] - Okay. I never knew that's what the name was. - Now you know.
[37:36] - We'll see if I remember that part, though. - Tilde, and we're going to do equals. And then we're going to, in quotes, write center text.
[37:52] Center dash text. And so, what this says is, hey, if somewhere the value that is given to data centered, if you can find that word center text in there, then let's do some extra styles.
[38:14] So, this way we can get, we can, anyway, you'll see the value of this in just a moment. So, let's do the curly braces after the square bracket.
[38:23] - All right. And Bakari said that not far from the truth, I think, about, you know, we found the holy grail of, you know, the centering for height and width. So, all right.
[38:37] Back to this. Okay. - Appreciate it. So, in center text, let's do text dash align.
[38:46] And then, yeah, give that a property of center. So, now we can go up to that data center there on line five, I think, in HTML.
[38:59] - Okay. - And let's give that data center and let's make that equal
[39:05] center text. Oh, you got to put in quotes. - Okay. It's not like I can type either.
[39:21] - There we go. So, now we're, just by adding that value, we can conditionally decide we want to also center the text. So, we can use that data center,
[39:36] maybe go add it back to that dad bot or whatever, one of those, like, jokes. And then, we want to do this. And then, we do data dash center equals quote.
[39:53] - Oh, no. Let's do space. And this one, because, and you can't, it's taking up 100 widths. So, we can't actually see that in the center just based off its content. But this one's not going
[40:08] to have the text center because we didn't add that attribute, but it still has all the other properties. So, this allows us to use that same thing and, like, really, like, customize how we
[40:22] use each one. - Okay. And that's why it's the unexpected error. - I wonder what that, I don't, oh,
[40:31] do you have a quote there still? - Not for data center. - Huh. I don't know where that unexpected error is coming from.
[40:39] - I'll retype it because I might have put the quote in. And then, why is there still an unexpected error? I just put you back to normal.
[40:48] I don't know. - Oh, that might, maybe that was a grammar release, like, complaining. I don't know.
[40:59] - Well, unexpected error is theirs. But if I double click on that, it tells me grammarly. So, I don't know. It's fine. If it works, it's fine. - So, anyway. So, that's one thing we can do.
[41:13] And if we want to have some other attributes, in this case, we want to maybe have, like, the children inside of it also to be centered. So, we can do that. Let's go back down on 63,
[41:32] and we'll find, let's copy and paste. Let's describe everything that we wrote before. - For 60? - Yeah. From 61 down to 62.
[41:43] Yeah. We have too many, like, curlies now. - How did I manage that? Oh. Because I did, there we go. - Perfect. But instead of center text,
[41:58] change that to center children. There we go. And inside here, let's remove that text-aligned center. And let's put display flex.
[42:20] Display colon flex. Sorry. - Okay. Yay. - And then flex direction center on the new line. Sorry, flex direction column. Sorry,
[42:35] my brain is, like, thinking one step ahead of the directions I'm giving you. - Flex direction what? - Column.
[42:47] There we go. And then align items. - Align. - Dash items. Uh-huh. - Dash items. Okay.
[42:59] Yes, flex box. We're going to find out. - Column center. - My dog is making really weird noises. Okay. - Okay. So, now we can go back up there to the
[43:16] that up above. Actually, let's do that to that article just so you can see what happens. Let's go equals. - And then do center children.
[43:29] - Yeah, center children. Let's just see what happens there. And then. - Oh, yay. It did it to it. - Yeah. So, you can potentially, like,
[43:44] center the children if you wanted to. Or you can do both. You can do center children space center text. And it will, because we did that tilde, it says it's going to take each of those words that
[43:58] we put in there and delimited by the space. And if it can find a word that says center children or center text, it will apply the styles. Your dog is really upset at you.
[44:11] - I'm going to go kick her out of this room. I will be right back. - Welcome. This is now my show. I'm going to say whatever I want because Jen kicked
[44:25] her out of the room. I'm just kidding. The fun of live TV, everybody. - The funs of. - Say some offensive stuff.
[44:43] - Whatever. Rude. - I should have said stuff like, by the way, Jen endorses everything I say. - I am learning a lot from everything you say.
[44:55] So, I appreciate it. Okay. Sorry for the rude interruption from my dog. All right. So, we were doing center children, center text. - And in this case, because the text
[45:09] isn't wrapping, you can't see that the text is actually a line center. - Okay. - So, let's remove it
[45:16] off that article because that's not how we're going to do it in the long run. I just really want to just show you. Like, let's remove all that data center.
[45:22] - Okay. - The let's go up. But just to make it clear what's happening here. Let's go back up to that div.
[45:36] And let's add that center text. Sorry, the data center. Let's do center children on that. - And do I do it inside of the quotes? - Inside of the quotes. Yeah.
[45:49] - Yeah. Okay. Cool. Center-children, right? - Yep. And then next. Next to, outside of the quotes, we're going to do a style.
[46:00] And we're going to define that max width. It's in quotes. Yeah. And we'll go dash, dash, max width.
[46:17] Colon. And let's do, yeah, 500 pixels. Why not? - And then let's maybe bump up the, or bring down the font just so you can
[46:34] see exactly what that's going to do. Still haven't seen it. Let's, I really want to make that text wrap. Let's change 500 pixels.
[46:46] Let's go. - I made it too big that I can't, like, see enough. There we go. 500 pixels to... - Let's go, like, 100 pixels. Let's just
[46:59] really exaggerate it. - Oh, that one's wrapping. - Yeah. That one's wrapping. Let's go back to the center, the data center in the CSS. Sorry.
[47:17] Let's make sure, max inline size. - Yeah. And just because I moved that up doesn't mean I wanted everything else to move. There we go.
[47:29] - Max width. Interesting. Let's give it, like, 10 pixels. Go back up to the, that max width where we were defining that. And let's give it 10 pixels. Let's just really
[47:45] exaggerate that. Right there. Yeah, it's not... -
[47:59] We have more that are doing it. - I am confused. We're doing dash dash max width. - I'm gonna make it bigger just to
[48:17] see if it'll... I mean, it's doing it now. - Yeah. I just wouldn't... It should be, like, like, really small max width there. Data center, max inline size, dash dash max width.
[48:39] Oh, on 59, we gotta put var in front of that. - Over here? There we go. - So, let's change
[48:53] that back to 500 pixels. I was like, that should have been, like, right. - Yay.
[49:07] - So, yeah, this is... So, now we can see how that's working. We can use the center now in any way we want. We can mix and match and kind of really customize it for the situation. Because
[49:21] sometimes we don't want text-aligned center or sometimes we don't want the children centered. We still want them to be left-aligned inside that box. But sometimes we want everything just,
[49:31] like, totally centered. So, that's what... It gives us all those options. If we can use just this one data attribute to cover all those options now.
[49:39] - Very cool. Very cool. And, I mean, there was a lot to learn here. But, like, at the same time, it's so intuitive. Maybe it's not. Maybe it's just... But I feel like so many people...
[49:53] - It totally seems like... We kind of, like, get really bogged down in the how we got there with, like, display flex and all that stuff. And we kind of forget... We don't see the forest
[50:07] for the trees kind of thing. And we really... What we're trying to achieve is this cover layout. And then a center layout. And we're composing those together to make this vertically and horizontally
[50:19] centered content. Anyway. So, that's why I really like to think of a web layout in this way. Also, because I don't want to sit there and remember every single time all these properties. I need
[50:30] to have this combination of properties. You can define it once. And now you can bring these into any project and just go, "Hey, this is a centered. And I want this centered. And I want this as
[50:41] using a cover pattern." So... - Okay. Now, we can either have 10 minutes left or 40 minutes left. Whatever you want to cover. Because I always schedule them for an
[50:54] hour and a half. But I think the attention span is like an hour. Although sometimes we get a little stuck and need that extra half an hour. Is there anything else that you wanted to make sure we
[51:07] covered today to do bedrock? That is what, Anthony, spin up bedrock. - Spin up bedrock. You want me to actually do it with bedrock itself? Just to make things... Just so you can see the
[51:22] value of using bedrock and not having to recreate these. Let's go into the settings up above there. And go to the CSS. You can see the CSS that's being imported.
[51:36] Scroll down on the right side there. And you can see I brought in... Keep scrolling. Yeah. So, right now, I'm using open prompts. And you can see I've got this bedrock layout. This... So,
[51:53] go down into there and you'll see bedrock layout CSS 2.0.3. And just remove everything after that. - After 2.0 point... - Yeah.
[52:04] - Okay. - And then close. And hopefully nothing breaks. Perfect. So, let's go into... Now we can just
[52:24] close the CSS because we don't need it anymore. We're just gonna live in HTML the rest of this time. - I don't even know how to close it.
[52:30] - Yeah. There we go. So, first thing we want to do in this main section, you'll see these, like, top jokes and then a whole bunch of, like, cards. And then there's another set of jokes.
[52:44] So, on main, we want this to be a stack. So, right next to the... - Real quick, I have... Anthony posted about what y'all did with JS jam. FS jam. Wow,
[53:10] I can't even talk today. And then explained styled components. You've abstracted it out, but still it's probably relevant to mention. - Yeah. Yeah. So, yeah.
[53:23] I was on Anthony's podcast, FS jam. And I think I'm due to come back on, right, Anthony? I'm just kidding. That was just a joke. - Like, two things that Anthony told me
[53:37] when I first met him were, don't worry about web 3 yet. He's like, you're not there. Don't worry. Unless you really, really want to. And then also, his podcast may be too technical at this point.
[53:53] - Right. - For me. And I was like, fair enough. So, that's why I'm always like, oh, yeah, he has a podcast because I'm not listening
[53:59] to it. So, yes, go back on. And then I will listen to the first one and the second one and see if I finally start to understand these things. - Yeah. No worries. So, yeah. The main version
[54:13] of Bedrock is built in React using styled components. Styled components is a library that allows you to write CSS and it gets it generates the CSS on the fly at runtime. So, as you so,
[54:28] you can basically, like, define, like, this is how I want the CSS to be built depending on the context. And then styled components based off the context that's actually being used builds the CSS
[54:40] as you go. There's there's some tradeoffs to that. But, like, for most people's apps, it's probably it's perfectly fine. Because you get some nice, cool benefits with that as well. You get, like,
[54:52] you don't have to download a separate CSS sheet and all that stuff. It just all comes in, then styled components builds it. - You do have a question from Bakari
[55:06] of what is the best way to become a badass at CSS in JS? - Use it a lot? I don't know. Just do a lot. Build a lot of crap. That's what I found.
[55:19] - He did say that he was going to take your course, for sure. And, yay, Anthony said I finally graduated to being able to listen to it. Anthony, you weren't here earlier,
[55:31] but I was telling Travis you're, like, the big brother that is, like, really... - Not big brother, like, 1984 big brother. - Like, very, like, you're going to do this
[55:43] and learn it in, like, a really caring way. Like, I think that's the best way of saying it. So, that way I, like, learned the best structure. I don't know. Maybe that made sense. But...
[55:54] - No. So, what we're doing here, though, is, like, an abstraction from the original library that was built in React and all that. It's just a CSS framework behind it. So, that's
[56:07] what we're going to be doing here. - Okay. - So, in main, let's have you go to main. Sorry. You were right there. Like...
[56:15] - Oh, okay. Yeah, yeah, yeah. Right here. - Line nine. So, after the word main, I want you to write the word data-bedrock. Oh, sorry. Inside the...
[56:25] - In the class, right? - Yeah. Data-bedrock-stack. Yep. So, by default, this is going to, like, stack everything
[56:40] inside that more violet-y, lavender-y section. But what we want to do is we want to put some gaps in there so we can see that content. Sorry. - Okay.
[56:54] - So, let's do style. - In the same area? - Yeah. So, go space, style, equals. And in quotes, do --gutter. Oh, gutter. Sorry.
[57:13] - Gutter. I heard scatter, and I'm like, I don't know if I know how to spell scatter either. - Then colon, and let's do, like, torem. M. Sorry. R-E-M. Like, the band.
[57:30] - Okay. - That should, assuming that it brought in everything, work. Interesting. Oh, let's see here. Stack. Yeah, that's how you spell
[57:47] stack. Data-bedrock-stack. What is going on? - It could be just a missing letter somewhere. I will tell you that. Bakari and I had to learn that the hard way. Instead of "payments,"
[58:07] I put "payment" somewhere. - Data-bedrock-stack. - Or no one out there. - Gutter. G-U-T-T-E-R. Yeah.
[58:23] Well, now I'm curious. Did it actually bring in this? - Do I need to go back to settings? - Yeah, let's go to settings. Let's see
[58:36] if it actually brought it in. - And then all the way down. - You might need to, like, so copy everything you have there,
[58:46] remove it, and then paste it back in. - Paste it in the one underneath. - Yeah. - Scrap that one. Close.
[58:57] There's not a save anywhere, right? No, there's no save. - No, in fact, the @.2.0.3, let's maybe get rid of that.
[59:07] - All right. Close. - Why is that not working? - It still says "unexpected error," and I don't know why.
[59:22] - Do you mind if we, like, if we look at the, debug the code? Let's go to that. So if you right-click on, like, "top jokes" in the HTML there.
[59:36] - Oh, and then inspect? - Inspect, yeah. - Okay, cool. Oh, I'm so excited. I love debugging because I'm learning so much.
[59:43] - Yeah, instead of "main," yeah, just highlight the word "main" there. Yeah, click it. And it is, yeah, the data bedrock stack. It's coming in there.
[60:01] Hover over on the right-hand side there, you'll see gutter. Go down there. - Click it? - Yeah. It's getting that to RAM.
[60:16] - Is it trying to read some of the CSS we already wrote? - Oh, I just realized it is probably working. I'm looking at the wrong thing.
[60:26] I'm not thinking of the data. Okay, go ahead and close this. I now not realize. Okay, scroll down from, like, the top jokes. Like, scroll in between top jokes and food jokes.
[60:40] There's two REMs between the word "food jokes" and that section of cards. Right... - Right here? - Yeah, right there. That's the two REMs.
[60:51] - Okay. - I had in my mind something different. Like, okay. So we're going to do the same thing again with this section.
[60:58] - Okay. - Let's do data bedrock stack again for... - In the section? - Yeah, in that section.
[61:07] - And then same style? - Style. This is the fun of live streaming. You get to see even, like, experienced people forget. And let's do one REM here.
[61:27] And it's a double dash for the gutter. - Oh, yeah. - And then... - There we go.
[61:38] - Now we have our spacing. Yay! - Yeah. And then let's do that to the other section as well. The same exact thing. So...
[61:47] So, yeah, right above food jokes, we'll do data bedrock. - Yay. It's so pretty. - Awesome. So the next thing I want to do
[62:12] is just show you how to do, like, there's the grid of columns. And we want to have, like, a responsive set of columns that will, like, take up as much room as they possibly can.
[62:22] But as it runs out of width, it will, you know, reorganize themselves. - Oh, okay. - So to do that, so on the...
[62:29] Around each of the articles. So let's go back into the top jokes. Yeah. Let's wrap that in a div. - All of them? Or just this one article? - All of the articles. Yeah.
[62:45] - I'm going to close this div. I was like, I have a feeling we're going back there, but I need to make sure to close my div. - Yeah. So write a... Oh, not there.
[62:56] One more down. - Before article or after article? - After article. Yeah. - Okay.
[63:05] - Not div. - Oh, you know what? I think I did the same thing up here. Oh, I did do div. Okay. So I have my div. Not div.
[63:16] - So we're going to use data bedrock grid. - Bye, Anthony. Enjoy lunch. - Have a good one. Thanks for jumping on. - Bedrock grid.
[63:28] - Yep. And we want to set the minimum item width on these. - Okay. - So let's do space.
[63:39] So let's do style. - Equals. - So actually, before that, let's set a getter. Sorry. In style. We'll still do style equals.
[63:52] - I found this on the web. - Stupid watch. - I don't remember how we wrote this one. - It's a dash dash getter.
[64:03] - Dash dash getter equals one? - Yeah, let's do one rem. And then do a semicolon. - Before or after the quote?
[64:20] - After rem. - After rem. - No, before the quote, after the rem. - Okay.
[64:25] - And then space, because we're going to define a second property here. And we're going to go dash dash min item width.
[64:31] - Oh, sorry. Item will be a capital. - Oh, okay. - Min item width. And let's see. I'm trying to think what a good size would be. Let's do
[64:58] two rem. We can play around with this. - Oh, cool. - Now, just so you can see what it's doing. Let's change that to, like, 20 ch.
[65:13] Now, ch, that basically means 20 characters. - Oh, what does rem mean? - Rem stands for root. The R stands for root. And I'm also, like, having a blank with the ems.
[65:33] But the ems basically means the font size. So, that typically means 16 pixels. But it could be different. So, if you're in a header, the ems are going to be higher.
[65:45] So, if you want things to be consistent, no matter where they are, even inside of header, you would use rems. So, as you can see here, if you go back up, as it's taking up,
[66:00] that each one of these boxes has to be at least 20. - I changed it to 25, the way I like to look. - Or 25 characters.
[66:08] But if they can take up more space, they will. They're going to try to put as many of these cards in a row as they can without making them smaller than 25 rems.
[66:20] And if that's the case, then they'll move them to another line. And, yeah, and you can see, like, as you move things around, it's going to adjust that and make them as wide as possible
[66:30] in each of these cases. - I got excited. Now, I want to do the other one. - So, the other one,
[66:37] we're going to do something very similar. - Oh, okay. I won't get too excited. - So, actually, let's just copy that. Let's just bring the whole, like, data grid over. So,
[66:46] yeah, let's do... - And let me make sure I get my other div. - Yeah. - Before I forget.
[66:51] Okay. - So, it's going to look cool. There's definitely a pattern for this, a style for this. But instead of doing grid,
[67:02] let's do something a little bit more fun. Change it to data bedrock column, dash drop. - Dash rock? - Drop, D-R-O-P.
[67:17] - I just didn't remember far enough. - Let's see here. And then let's pull it out. Let's make it a little bit wide. No, not pull it out. Sorry. Let's make
[67:35] the screen a little bit wider. These should be, like... - Oh, that's cool. - So, it kind of does the same things as the grid. But instead of, like,
[67:48] those columns, like, translating all the way down to all the rows, each time the content drops to a new row, the columns reset. And that's why I call it column drop. So...
[68:01] - Oh, this is fun. - So, yeah. And maybe change this one to 20 CH, just so you can set a minimum item with 25. Let's change that to 20, just to see.
[68:14] Interesting. Yeah. Basically, like, once it gets to a certain point, it's just going to stack everything. And in fact, both of those... - There we go.
[68:26] - Yeah. - I just needed to make it a little smaller. - Perfect. There we go. Let's do the 20... If you want to do the 25, that...
[68:37] - It does it if I just move this, right? It shows the difference. I like that. Because it shows, like, right here, how it just does... This one's the largest. It needs to take
[68:49] up all the room. - Yeah. - This is cool. - So, we could have
[68:56] recreated all these ourselves and shown you, but this is what my library gives you, is that you can just use these layout patterns automatically by yourself. You don't have to think about recreating
[69:05] these. You can just go, "Oh, I want to have a grid pattern here. I want a column drop pattern here." And there's a whole bunch of other ones in there as well.
[69:12] - This is so cool. - So, that's the idea of this, is just to help you, like, not have to, like, think about, like, layout. Like, you just, like,
[69:22] think about, like, what you want to do. And then this library helps you achieve it. And then you can get back to, like, making it pretty and doing all the other things that are fun to do.
[69:30] - Okay. So, last question before you go. How did you end up creating this and deciding to do this? Because it's really cool. And that's my curiosity question.
[69:43] - It's a crazy thing. So, I've been, obviously, like, working on this for stuff in the industry for a bit. I was specifically, though, part of a design system team at a company called R1.
[69:55] And we were building our design system and component library. And I wanted to get permission to open source it. And I couldn't. And so, this is a short story. Like, basically, I'm, like,
[70:10] well, I'm going to show you. I'm going to make an open source library anyway that does some of these, not everything that we were building in the design system, but just the parts that I was having the
[70:19] most fun at the time building, which were these layout patterns, these component patterns. And the, yeah. And so, that's what I did. I built it out originally using just reaction style components.
[70:32] And as I've gone, I've just continued to, like, just find new and more fun ways to, like, just keep building this. This is where the CSS library now has come from.
[70:42] >> I dig it. This is really cool. And thank you for coming on today. Because this taught me a ton and actually made it not seem as scary to build a website.
[70:52] >> Good. >> At least on the front end. Eventually, Anthony taught me about making a React app with Vite and Bracel. And then Ramon taught
[71:06] me about making an API with Express. And I'm like, between all of these, I'm just going to be able to make a whole web app. >> You're just going to be, like,
[71:18] the master full stack app developer. >> Eventually. Eventually. I need to go watch all the old ones and be like... >> You're going to have to change the
[71:26] title from "Teach Jen" to "Jen Teaches You Shit." >> I know. No, no. I'm like, I have a podcast called "Shit You Don't Want to Talk About." I'm like, whatever.
[71:35] Yes. And that's a big thing, I think, is something that's so cool about the tech community is it's like you learn, build, then teach. And you always pay it forward. And that's a big reason I wanted
[71:50] to learn these live is because it gives somebody an idea of where it was, you know, to start with something. And then eventually I'll be building more instead of learning as much. But there's
[72:03] still so much out there to understand that I'm like, I don't even know what direction to go in yet. >> Oh, and you're always
[72:09] learning. There's, like, things I was just, like, learning about today, just before the stream, working on stuff at work, that, like, it was a situation I've never run in before. And it was,
[72:19] like, you're like, oh, I can do this. This is something that exists. And maybe it didn't exist two or three years ago. And that's why I didn't know about it. So, yeah. That's what I love about
[72:30] this industry is that, like, you're never going to be caught up. So, there's a little bit of anxiety for that. But there's also a lot of fun. Because you're always learning. And I love the
[72:38] always I like to look at it as I'm always learning part of it. >> I dig that. And I think that is also something that I do appreciate that Anthony is always telling me about documentation. And
[72:49] I'm also going to have R4DZ. >> You've got a family this whole week. >> I know. R4DZ or M4DZ is going to be coming on and teaching about documentation, too. Which
[73:03] I think that's going to be so important as to when you have to learn something new of being able to understand how someone goes through and does it. Because for myself, something I've always
[73:15] struggled at is somebody would be like, okay, go do this. Here's instructions. But it doesn't always make sense without being able to see someone do it or, like, be able to ask questions
[73:27] like today. So, I really appreciate you going through and just Twitter makes things so accessible and so does Discord. There's so many Discord and Slack channels and communities that
[73:41] people you can do tech. It is possible. >> Yeah, there's some crazy gatekeeping tech people. But I say most of them out there all went through a lot of crap to get where they are and
[73:56] they know how hard it was. And like you said, they want to pay it forward. Even if they aren't full time mentoring, most people I know are totally willing to, like, answer questions, help people.
[74:07] Like, tech Twitter is so much more approachable than most people even realize. >> Agreed. And I will say something that may give people, like, that idea that they don't want to
[74:19] teach is the fact that it's not necessarily they don't want to. They don't understand how to explain it or have the practice of how to explain it to a newbie. >> Yeah. Teaching is a feeling of
[74:30] itself. Exactly. >> Yeah. So, thank you once again. And I don't know what you'll be coming on the show again, but I'm definitely going to be hitting you up after I understand stuff more. So, maybe a
[74:44] month to six months, I'll be like, yo, Travis, you've got to come back because there was a lot of knowledge dropped today. And I appreciate that. >> Well, exactly. And you'll probably get, like,
[74:53] remember 10% of what you learned today. >> That is why they're recorded. >> Exactly. But 100, hit me up anytime. >> Awesome. Thank you, Travis. Bye, everyone.

