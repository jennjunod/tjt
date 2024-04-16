---
showLink: "https://www.youtube.com/watch?v=8vGeKR8w35g"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-is-this-accessible-with-graham"
title: "Teach Jenn: Is this Accessible? With Graham"
publishDate: "2023-11-11"
coverImage: "https://i.ytimg.com/vi/8vGeKR8w35g/maxresdefault.jpg"
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

[00:00] Oh, right. That's always fun. And hello, hello, beautiful humans. Welcome to another episode of Teach Gen Tech. And we have Graham, the dev, on here today to talk about accessibility.
[00:15] I'm curious, as we let people join the stream, what people thought about our graphic that we posted and accessibility. So we'll give some time for people to wander in. But to
[00:31] get started, Graham, who are you? So yeah, thank you. First of all, thanks for having me on the stream. And secondly, hey,
[00:38] everyone, I'm Graham. I'm doing accessibility now for over 10 years. Software developer for over 15 years. But I ran my own business for a lot of that. So I was the one who was
[00:52] looking after developers, and they did the hard work. And I just told people what to do. It was a much better way of doing things. You should all do that instead.
[01:00] Recently, I stepped away from the business about three years ago, worked at Daily Dev for a while. And then this year, I've just been having a bit of a float around and everything
[01:12] on the job hunt at the moment, stroke, setting up Totally.dev, which is a business around accessibility as a service. So yeah, that's me in a nutshell. But anything accessibility,
[01:22] love it. Anything performance, I also love that. That was the main core part of the business that let us upsell. The accessibility was all around web performance and load time.
[01:33] So you'll often see my face pop up whenever you ask a question about, for example, Google Lighthouse or PageSpeed Insights. I did a lot on that one. And hey, to all the beautiful
[01:45] people who've joined us. Yes, yes. And thank you for the follow. And I do want to call out, Jason, how is it that
[01:53] you just followed like 56 minutes ago? That went in like WTF. Poor, poor Jason, already getting abused. He's only been here 10 minutes.
[02:10] Yes, yes. And I just wanted to call out because, okay, Ben, I messaged you about the stream today and then like, oh, I'm putting myself on blast too. And then I'm like talking to
[02:23] Graham afterwards. And so I told Ben, I've never had anybody on the show for accessibility. And I was trying to say, I haven't had anybody on the show for accessibility since Ben. And
[02:37] then it came back to me telling Graham, oh, because you've been on the show before. And I didn't mean it like that. He's just like watched an episode or two that I'm like, you
[02:47] know what, words and I. And I just want Jason to be there as well. That's just what I'm doing today.
[02:54] I mean, by the end of this stream, hopefully we'll have offended absolutely everybody. And that means it's been a successful stream.
[03:02] Touche. Touche. Yes. That should be the goal. That should be the goal. And thank you, Todd, for following. And yay. Okay. I'm curious. So for everybody that if you didn't see the
[03:21] social media posts about this stream, let me show you a few things. Because we had a question that really set up this stream. And also what I learned from Ben, I think almost
[03:38] a year ago, which is really crazy to me. I can't believe it's been that long. Of is this graphic accessible? Helps if I zoom into the right screen. Oh, look, it has 777 views.
[03:54] That's kind of fun. Let's do that. And I will share it right here. I am curious what y'all think. Is it accessible? Is it not accessible? Why or why not? And just so that way y'all
[04:11] know, the alt text is upsetting. Yes, but deliberately so. It's one of the few times where I'm happy that you put that
[04:24] alt text on. I'm not going to cry too much about terrible alt text today. And Elian. No, no. Elian. Elian. Elian. Dude, you've been on the show and I still can't
[04:41] say your name properly. Oh, my God. I correct myself like seven times still while doing this. We talked about maybe looking at my website. And I'm like, well, it was a thing
[04:55] that I really broke and never fixed. And I'm rebuilding my site again. So, I don't know if... That's great. I said we probably shouldn't do that. And Ben... Oh, the bottom text is
[05:15] a little thin for readability's sake. All right. All right. Anybody else? What was your thoughts, Graham?
[05:25] I had a similar thought. I did try and do a contrast check on it. And ironically, it's pretty close to passing. There's a couple of light parts behind the text. But ideally,
[05:36] that text at the bottom would have been whiter, lighter, and probably had a background behind it that wasn't as fussy. Because that fussy background can be very off-putting.
[05:45] However, other than that, the image itself is pretty decent. The text is a half decent size. There's good contrast on the learning from Graham about web accessibility part.
[05:58] You know, it wasn't bad. Your alt text was the bit that made me cry. But deliberately so. So, you know, that's not the end of the world. I know why the alt text was not good.
[06:08] Let's look at the alt text. For those who may not know, alt text is where when you need to use a screen reader to be able to read what's going on if you're unable to read it.
[06:28] And I... Ben, I know. I know. I know. I purposely did this one. I knew it would make you mad, Ben. It's really funny. I forgot to tell Ben about the stream until today. And also, what
[06:43] up, cat? I was trying to reply and open Twitch up. Yeah, it's just not working. But yes, alt text is for a screen reader for when you want to... Something needs to tell you about
[07:01] what the graphic is. Or a picture is. Instead of it just saying "This is a picture." >> Not a bad description. Not a bad description of alt text. It's the context of the image
[07:13] and the important information. The easiest way to think about it is always to imagine if somebody is blind and using a screen reader. It's not the only reason why alt text is important,
[07:25] but that's the easiest one to understand. You need to, in context, explain all of the important information of that picture. We always say, imagine you're having a phone
[07:34] call describing, in this case, the post. What would you tell people that's important on that image? And so, obviously, the text is important, and then you may want to say a
[07:44] little bit about the abstract background. But other than that, like the fact there's a red background behind the white text, is that important? No, not really. So, you'd
[07:54] probably exclude that sort of information. >> And thank you for that. And y'all, I just want to say, like, life goes full circle. Because not only do I have, like, Renee hanging
[08:06] out with us from GoDaddy days, which was, like, dude, I haven't worked there since, like, 2018, 2019. But James is here. And I knew James in high school. And I don't want
[08:18] to say how long ago that was. But we knew each other in high school. And it's just really cool how, like, when you work on cool things in life, how it can, like, wrap back around.
[08:30] So, just wanted to say hi, y'all. And yes, that is a great, great way of explaining it. And what about SEO? Are you supposed to use it for SEO?
[08:43] >> Ooh, the leading questions that you know that are going to make me upset. You're trying to make me angry. I like it. I like it. No, please do not use your alt descriptions for
[08:53] SEO. That is not what they are for. And to be honest with you, it won't even work anymore. There was a point in the past where keyword stuffing in your alt text was a thing that
[09:03] would actually work. Nowadays, it doesn't. So, don't do it. It's not what it's there for. It's to help people who need that information to be able to enjoy your content.
[09:14] And also, for people who have images switched off, people don't think about that. But there's a lot of countries out there where data is expensive. They may browse with images blocked.
[09:23] It gives a description of what that image is so they can decide whether to unblock images if they want to see it or not. So, that's another reason why you should use alt text
[09:31] to describe the image, not to try and stuff 50 keywords in there. >> Okay. Y'all, I'm going to pick apart my own just social media side of things, like
[09:44] graphics you should or should not do because I feel like this is a great way of learning because I guess before I do this and I'll remove my screen for a second of why, like,
[10:01] we're talking to a lot of developers. We talk to a lot of people that may be coding, but they may be, you know, just social media in general. They may, you know, just why is accessibility
[10:13] important to all of us instead of just screen readers? Because all of us end up temporarily disabled. The situational disability that people completely
[10:24] forget about. But, like, bright light on your phone. You know, bright light shining on your screen. I always give this example. It's such a good one that everyone can appreciate. If
[10:33] you've got poor contrast, so, for example, that text that we've all been complaining about that's very thin and not great contrast, if a bright light's shining on your phone
[10:41] screen, you're not going to be able to read that. So, color contrast in that example and enough contrast between the text in the background would mean that in a bright light I've got
[10:50] a better chance of being able to see it. It's also things like maybe you've got a young child. Maybe you're having to work one-handed,
[10:58] so have you thought about that? Because that's exactly the same as someone who may be an amputee. They have the same disability. It's just that yours happens to be situational
[11:08] and temporary, whereas theirs is permanent. That's the only difference. You still have the need. You still have the want. Accessibility benefits everybody. The main thing that's
[11:19] important to remember, though, is some people need you to think about accessibility, and some people, they can cope without it. They'll just look at it later or something. I think
[11:30] it's a real shame that we are so far into this world and we still have people who are being excluded just because people don't talk about accessibility and teach it. So, devs
[11:41] make terrible choices, and their choices impact thousands to millions of people. So, there you go. There's me getting on my high horse. I'm sure I'll be up on it a few more times
[11:53] before the stream's done. That is okay. That is something. So, funny enough, Graham and I talked about this a little
[12:00] bit beforehand. I think we met in Twitter spaces. I've had TeachGen Tech for about a year or a year and a half now. And yo, it's Yuri! What up? And Jason, what is going on?
[12:18] Oh. It's interesting because, like, something that I learned that I'm still learning, this is not something that is done, is when you try to please everyone, you please no one.
[12:33] And when I first met Graham, or knew of Graham, I didn't understand his humor. So, I was like, what is wrong with this guy? But now all the -- but no, it's so -- I really enjoy the humor.
[12:48] And I love that you just, like, you stick to where you are, like, who you are. Because being polarizing, like, the people that are meant to be, like, in your bubble are going
[12:59] to be there. Because if you're pleasing everybody, you're honestly not going to make yourself or anybody happy. And I find that just really funny when we're talking about you going on
[13:08] tangents and things. Because I'm like, I appreciate that. That is something I know Graham will do. And why I asked him to be on the show. So, ooh.
[13:20] We could end up on some very large tangents by the time we're done. But that's half the fun of winging it as we go.
[13:26] >> Yes. This is a very winging it episode. A lot of them I have a game plan beforehand. But this one, I'm like, we got here. And sometimes that's, like, the best you can do. It's, like,
[13:36] the days when you're having a rough day and you just, like -- it's a win just getting out of bed. So, we're having that kind of stream today.
[13:45] And James said -- they always look at it from the position of that health isn't static. Good points. Access, whether you use it or not now, benefits everyone. Helps bridge gap
[14:01] between those with or without access. With access and those without it. See if I can read. Which is actually a really interesting thing. Because I would say, yo, StreamYard,
[14:14] I am going to call you out on this. It's not very accessible. I can't, like, actually hit the text in here without bringing it on screen. And if I wanted to hear the text from a screen
[14:25] reader, I can't highlight it to do that for me. Because I'm dyslexic. This is a big -- one of the episodes with Ben was a lot about screen readers and text-to-speech. And I just pasted
[14:42] those. A, I didn't know there was a difference. And B, like, it's these type of things that also are part of accessibility. So, all of that said, when somebody is building
[14:56] a new site, like, let's say that they want to build a new site or they want to start looking at key features of anything that they're working on, what are some -- would you say
[15:06] are the five top things somebody should look at when building an accessible site? >> It's an interesting way of phrasing the question. I'm going to go back a step, actually.
[15:20] Because that comment was really interesting. Because it lets me tell the story of how I ended up in accessibility. So, I'll take the opportunity to share that story. Many people
[15:30] have heard it before. And then it gives me time to formulate my answer. So, yeah. Temporary disability was how I ended up in accessibility. I fell down a flight of stairs. And hurt my
[15:43] wrist. And was looking up how to do, you know, like, Control-Alt-Delete one-handed and things like that. And came across sticky keys. Which is, you know, it's a very simple thing. But
[15:54] a lot of people may not be aware of it existing. And then I fell into this wonderful world where it's like, oh, accessibility matters. Oh, there's a lot of people rely on it. Oh,
[16:04] wow. Oh, it's interesting as well. And that's how I got so invested in it. It was literally a trip. And like I said, it was only maybe six weeks where I was struggling. But it sparked
[16:18] this passion that is now ten years, probably, that I've been doing accessibility stuff. Because I realized my code has impact on people. And it matters what I do. And sticking to
[16:29] standards is important. Anyway. I got on a tangent with that. But I like telling that story. Because a lot of developers are a lot younger. Probably have an experienced disability.
[16:39] That was my background in life. I didn't really know anyone with a disability. Or at least not things that I'd actively thought of as disabilities. You know, I knew people who
[16:50] were colorblind. I knew someone who had... I don't know the proper term for it. So, excuse me here. But he had interned legs and had to have them corrected. So, I did know people
[17:01] who had disabilities. I just never thought about it that way. And I never really thought about... Oh, how on earth does someone who's blind use a website? How do deaf people interact
[17:11] with... You know, have a phone call with somebody? These are the things that I just... They weren't on my radar. Because nobody had the very simple thing to say it to me. And so, that's why
[17:21] I'm now so invested in it. It's for me to spread that same message to people who may have no clue. And it only takes one person to go, "Have you thought about this?" And
[17:31] then all of a sudden, some people go, "Oh, wow." And then they get interested and invested. So, that was my tangent to give myself thinking time.
[17:39] >> I like it. I like it. If you're open to it, I'll give you a few more moments. Because I think that was something really relatable. And we can wrap back to the top five things.
[17:51] >> Okay. >> Okay. Okay. I think... I feel like that is... It is very relatable. Because for many of us, and something that... A big reason
[18:03] I started TeachGianTech was, yes, to get into DevRel and get some content and learn tech. A lot of it was because tech isn't very accessible in general. And we're not necessarily talking
[18:18] about the... You know, using the technology or those type of things. But also the communities around it and the knowledge isn't as accessible. And that was something that was very important
[18:34] to me of wanting to level the playing ground. And something that I appreciated... Ben... I think it was Ben that called me out. Like, told me this. Called me out. I mean, just
[18:48] told me this very kindly. That tech... Not everything... You can't make everything accessible. No matter what. It's something that isn't possible. But there are ways that you can
[19:10] change things. And taking it one step at a time. And doing what you can. A big part of that was because I had to pause my podcast to be able to keep up with TeachGianTech when
[19:25] I was job hunting and then getting a job. And having... Learning that lesson, I feel like I see so much more of, like, the work you do, Graham. And sticking with accessibility.
[19:43] Instead of spreading yourself too thin and doing nothing, you're focusing on something you can make a difference with. And that is a lesson I still struggle with of sticking
[19:52] to, like, staying focused. I have you so fooled if you think that I am very focused on accessibility. I try to make it the primary thing I talk about. But trust
[20:01] me, I'm like... Ooh, squirrel! And I'll go off and look at something interesting. And then I'll come back to it all the time. It's my guiding principle on things that I do.
[20:11] But I literally released an article the other day. And the solution... The thing in it was not accessible and there's no way to make it accessible. I'm still okay with releasing
[20:22] those things. Because they are exploring things and I explain what it is. But there was no physical way to make the actual end product accessible. Because I was abusing CSS and
[20:33] doing things you weren't meant to do with it. The thing with accessibility is you kind of have to follow the patterns that have been established to make things accessible. And
[20:41] when I was using CSS to build a neural network, there was no way to make that accessible for people. >> Interesting. There's a lot of layers there.
[20:51] What is... Well... Okay. What were you working on? And can you tell us about those, like... Frameworks? I don't know if framework was the right way that you... The right way to
[21:06] say that. Of how you said that. Because I feel like that goes into the five as well. >> Right. So... First things first. The article was a dumb, silly article. It was just a stupid
[21:19] idea I had. How far can I push CSS? So I've done bubble sort in pure CSS. No JavaScript, nothing. It was bubble sort in CSS. And then I thought, hey, can we push it a step further?
[21:32] Can we create a neural network in CSS? It's not what it's designed for. So that's where the problem is. But it gives a very nice parallel with a lot of the problems we have in accessibility.
[21:41] Which is people will use one type of element and then try and mold it to do something it wasn't designed to do. Prime example being a div as a button. You know? People do that
[21:53] all the time. Or href equals hash. And then that's a button. Even though it's not a button. It's an anchor. And it's really important to use the right element for the job. So...
[22:05] When you go outside of what things are intended for, you make it very hard, if not impossible, to make things accessible. And there was a point that you made there that Ben brought
[22:15] up and every accessibility person will say this. Which is... There's no such thing as fully accessible. There's just as accessible as possible. Within the limitations of technology.
[22:27] And also ability. You know? If you have a course on advanced mathematics and someone has a severe learning impairment, you will find that very difficult to make it so that
[22:37] becomes accessible. No matter how hard you try to change the subject matter, the subject matter may be something that will never be accessible for that person. So our aim is
[22:47] to improve things to a point where as many people as possible can enjoy them. Whether that's changing formats, adjusting the way you approach it, using simpler language. Which
[22:58] is why I brought up the cognitive impairments. Because so many people like to sound smart when they're writing and don't think of the fact that that's an accessibility issue.
[23:08] So there's loads of elements there. And so that brings us nicely on to... What am I thinking about when I'm building a website? That was your question a few minutes ago. And I don't
[23:20] think... So do you know about WCAG? Have you heard of the Web Content Accessibility Guidelines? >> I want to say yes. Because Ben was on the stream and he probably told me about it. I
[23:35] don't remember, Ben. >> Okay. No problem. So WCAG, there's many ways that people say it. WCAG, W-C-A-G. It's the Web Content Accessibility Guidelines.
[23:49] It's a set of the core success criterion, which yet again, we'd like to use fancy word. So a load of principles, guides on how to make things accessible. So for example, one
[24:01] of the rules is non-text content, which includes images and things like that. And controls. How do you make sure that people who cannot see the physical item can still access the
[24:15] same information? And that's essentially what an alt tag is. It's non-text content. It's a picture. And your alt text, your alt attribute text... Sorry, Todd. I said I would say alt
[24:27] attribute text just so there wasn't any confusion. That is there to give a text alternative that assistive technology can use to describe that image. That's what it is there for.
[24:40] So these 88 rules, I'm going to call them, as they are now, even though they are success criteria and guidance, are the founding principles of accessible design. I bring that up, ironically,
[24:54] to say that that's not the way I think when I'm designing something accessibly at first. They are the thing I think about later. The first thing I'm thinking about are different
[25:03] ways that people will interact with a page. So I will think about a screen reader. I'll think about people who rely on a keyboard who can't use a mouse due to dexterity issues,
[25:15] for example. And I'll think about how will someone interact with each element on the page as I build it.
[25:22] So if I'm building a header for a page, I'll be like, right, can I get to that menu with a keyboard? Yes or no. So I'll do a quick tab test, and I'll tab around and see if I've
[25:32] made any mistakes, especially if that menu has a dropdown. Can I open that dropdown menu with a keyboard? You'll be amazed how many websites you cannot do that.
[25:44] Then I'll be thinking about, OK, have I marked this up correctly? So am I using semantic HTML, which I hope you have covered at some point. But if not, we can cover semantic HTML.
[25:55] We should probably cover that again, because I don't. I don't. Y'all, I have over 100 episodes. I've learned a lot over the last year. I don't remember it all. So I'm saying that as a
[26:08] presenter. Ben, if you taught me this, I am slowly going back and indexing all my old stuff. But yeah,
[26:14] please tell us what it is. So you're probably aware of it without perhaps knowing the term for it. So it's things like
[26:22] using, instead of divs everywhere, you might use an element like main for the main content of the page, or header around the header, or nav elements. So I don't know if you've
[26:33] come across any of these or been taught around these elements. Yes.
[26:37] I don't know if I've been taught around them as much as using Astro on-- I've done two themes with it. Like, I built out one site completely, which was-- you mentioned earlier
[26:50] about having something that you're supposed to not completely morph into something else. I've tried doing that twice, once with a theme that I don't know whose theme it was. And
[27:03] then I fell in love with Alien's theme, and also tried doing the same thing. So I started learning what I'm supposed to be doing with them, instead of trying to create a new wheel.
[27:15] Is that the phrase? Yeah. No, well, it works for me. Even if it isn't the right phrase, it works for me. OK,
[27:24] so we should step back then. Like, semantic HTML is the basis, the foundation of making things accessible. And the reason we call it semantic HTML is, within those elements--
[27:35] so like, for example, main element-- there is extra information that is exposed to assistive technology. So that's the semantics. It has semantic meaning.
[27:48] So if you have divs everywhere on a page, when assistive technology tries to parse that page out, it has no information about that page structure. It has no idea what different
[27:58] elements are for. There you go. Here's a prime example. So on the left, we have our typical div soup, which you'll find in a lot of tutorials and
[28:07] all sorts of things on the net. And then on the right, we have semantic HTML. And so the difference is, when I approach that-- and yet again, the screen reader is the easiest
[28:17] way to explain this for someone to visualize. On the left, it will just say div, span, div, div, div, div, div, div. At the end of that, do you have any idea what that page is about
[28:29] or what any of the sections is? No. There's no information there. On the right-hand side, as I go around, I have landmarks that I can, A, understand what
[28:39] that's for. So it will say header. I know what to expect in a header. I'm likely to see a logo. I may see some navigational items. Brilliant. I know what that element is.
[28:49] And then I get to a nav. Amazing. There's going to be some links in there, maybe a couple of buttons, depending on the weird design of the website. Hopefully, mainly links.
[28:58] Aside-- OK, this is supplementary information. So this extra information is vital if you don't have visual information on the screen. I can't visually see this layout. So I have
[29:10] to be able to conjure it up in my head. And so that's what semantic HTML is there for. It's to let me know how to get around a page. And the added bonus is, once I've got familiar
[29:22] with that page-- so say this was an application you'd built-- I can use those landmarks with assistive technology to jump around the page, the same as you would just move your mouse
[29:32] from one side to the other. You can't do that if you're using a keyboard. So the semantic HTML lets me go, right, I want to jump to the article. I can bring up
[29:41] a list of all article elements on the page. And I can jump to one of them. So it aids with navigation. It aids with familiarizing myself with a page.
[29:49] Sorry, go on. You were going to say something. It's two parts. Thank you for explaining, because that was really helpful. And also
[29:59] thank you for comparing the two visuals, because that really helped put words to the visuals and how alt text may show up.
[30:08] What's popping out to me right now is understanding does header one, header two, all of those go into semantic HTML. That's part one.
[30:24] But also the other part of it was there was a live stream I had at a very random moment where I had 12 people on my live stream at once. I was coding while they were all hanging
[30:37] out. And Jess came on to the stream, and I remember her talking about something about like design defaults, like mobile, like if you click a button, it's supposed to react
[30:55] a specific way because the design tools say everybody needs to be doing very similar things. It's probably something like designing an iOS app. So there are some from Apple, especially
[31:08] from Apple, there are some very strong guidelines on how certain UI elements should behave and even be presented to an extent.
[31:18] That is very closely linked to accessibility, because one thing that's a very hard one for people to get their head around is expected behavior. So like if I see a certain element
[31:30] and it looks like it's a date picker, then it better behave like a date picker. If I click on it, and suddenly it brings up some new funky design that you've come up with
[31:39] that's really out there and out of the box, that is an accessibility issue. And that's for everybody. It's just for some people, it can be a lot harder. Like I see
[31:48] a new type of date picker, I have to work out how do I jump ahead a year? How do I jump back a year? How do I get to the next month? It's cognitive load. So that's why it's important.
[31:59] That's why more than likely, I could be wrong, they were talking about iOS, because iOS has very strong guidance on how UI elements should behave so that people can use applications
[32:11] more easily. I could be wrong. It could just be an internal design system. You never know. I'm Googling it at the same time. And thank you, Todd, for what you posted. And this is,
[32:28] I do want to say that I'm not trying to call out StreamYard and just keep throwing them out under the bus. I'm trying to use examples. Because if I click on this link to try to
[32:40] go to the link, I can't actually get to the link from StreamYard. I have to, and you talked about cognitive load, and also what the expected outcome is,
[32:53] is something that I think, I agree, a lot of people don't think about. Because while I'm listening to you, if I want to put this on screen, I have to make sure Twitch is open
[33:04] in another window, then copy and paste it. And I'm just like, what? Okay, hopefully I'm staying up to date with the conversation, and remembering what you're saying enough.
[33:20] And this is just a great, I'm excited to look into this later on. And I mean, I looked at Alex, I looked at your comment very, very briefly, you might have already left, which
[33:35] is totally okay. I totally get that in and out. But I'm like, for some reason, I thought it said like, see you, Todd, and Jen, and Graham. And I'm like, are we saying that we
[33:47] are like, all going on the stream at the same time? If we do that, y'all, we have to have Ben as well. Like, we could just, the four of us could just have a conversation about
[33:58] this. I don't know. I'm just totally spitballing here. But it's interesting to see all this, this does help. And I think it is very interesting. Also, something I noticed about myself is
[34:13] I get stuck on trying to figure something out. And I think it's like, UX design guidelines or something.
[34:21] Probably. Yet again, a lot of those guidelines will have, or hopefully will have, should I say, a foundation in accessibility. Because whenever you're trying to design a UX design
[34:34] system or any principles like that, it's the designers got a reasonable amount of the responsibility to consider things like, do we have space for visible labels on inputs? Is the color
[34:49] contrast okay? What will the flow through this particular workflow be like? Have we thought of that? Do I have, I can give you a good example. When I worked at Daily Dev,
[35:01] we had a notification system that we put in. So like when you upvoted something or left a comment, a notification will pop down from the top, a nice little toast. That was timed
[35:13] and there was no way to stop that from going away. Which is fine for most people, but if you're using a keyboard and you want to, you know, using assistive tech and you want to
[35:21] get to it in time and you want to read it properly, you can't do that. Or maybe you're in the middle of something at the moment and you want to take the time to read it later.
[35:30] So I brought that up and one of the things they implemented was an option to make it so that they don't auto dismiss. Very simple, but for some people can be very, very important
[35:40] because now that person could take their time to read it. And especially, this is like the added benefit, there's an international audience on Daily Dev where English is a secondary
[35:50] or tertiary language, a third language. So being able to have extra time to read things is reassuring for people instead of them rushing through it and going, what did that say? Was
[36:00] that important? I don't know. So it's, this is why I always say accessibility benefits everybody. Because by introducing that feature, it meant that everybody can switch it so that
[36:11] those don't auto dismiss and that could be useful for any reason. You brought up a great thing that at least related to my life, that the company I work
[36:24] for is an international company and the majority of the people I work with, English is not their first language. And if there are a lot of North American humans on a call, we can
[36:42] all talk very quickly because we go English to English. It's very easy to jump into it where it can take somebody that English is their second language a bit to translate and
[36:53] then be able to catch up. And this made me realize A, to give more pauses and B, to also talk slower. Yes, I still get excited. Like when I get excited, I talk really fast and
[37:09] I know that it's still something I struggle with. But my grandmother was like, you finally learned how to talk slower. I was like, but not because you said so. It was because...
[37:25] The ironic thing is I feel very called out because whenever I'm talking about accessibility, I get into my little zone. I forget that we're talking to an international, in fact, I forgot
[37:34] other people were here for a minute then. I was just chatting to you. And yes, I felt called out then because I was talking very quickly. So I'm going to now have to go back
[37:43] into my conscious effort, like I do in Twitter spaces, to talk more slowly and with more enunciation. So I liked that point.
[37:53] James just brought up another good point. And I find this is interesting also for the tools you choose to use. While this is primarily a conversation of tech accessibility, from
[38:09] their perspective, from the deaf, HOH transcripts and captions when using video/audio content, which also helps ESL people as well. And I completely agree. I think this is something
[38:25] that hits home for me because it was a the cognitive load to be able to use like a tool that would make this happen will stop could stop me from actually streaming and putting
[38:51] out this content and to try to learn this tool, even though I really want that tool to be there. And that's something that I think is just my own internal struggle of I would
[39:05] love to use OBS and ping. And there is a lot of like tools out there that are in my mind a lot harder for me to learn and take time to learn and test out while trying to keep
[39:20] up with just having my streams out there and those type of things. And I think that is something that is a really important conversation because it's something that I'm glad accessibility
[39:33] gets talked about in general because this is what's going to change tools to be made this way overall instead of me choosing between two tools to one that's overly technical to
[39:44] set up and use to one that is just a couple of clicks of buttons. So I like this conversation because I can give you a good example of where there was
[40:00] a huge improvement and that was on X Twitter. So originally trying to add an alt text there, sorry, alt attribute text, sorry, Todd, was like something you had to consistently think
[40:13] about and actively think about. Whereas they changed the interface very simply to say, hey, you forgot the alt attribute. You forgot to put some alt text on this image. And that
[40:22] little prompt has massively improved the amount of alt text out there. Now, unfortunately, most of it is garbage because people haven't been taught how, they missed the step of telling
[40:31] people how to write good alt attributes and alt text, but it was a step in the right direction. And it leads into what you were saying about why doesn't Twitch just have something built
[40:42] in where you can press one button and captions are generated on the fly. We have the technology. It's been there for many, many years. It may not be perfect, but it's better than nothing.
[40:54] And it helps people who A, I may want to listen to your stream with you on mute. And I know that won't be listening at that point, but I'll be watching, but you know what I mean.
[41:04] So I can still enjoy your stream while I've got you on mute. Perhaps I'm in a library or on a train or something. And secondly, obviously for people who are deaf or hard
[41:12] of hearing, it means that they can enjoy your content as well. One trick I normally do, and I presume using StreamYard, you can do screen captures of particular parts of screens.
[41:24] Are you able to do that? Maybe now that it has the web layouts, like when I started using StreamYard and a couple
[41:36] things to go into that one. Thank you, Todd, for adding this link in here for stream closed capture. This actually goes a bit into start using it today. So it only does Twitch video
[41:52] on demands or OBS WebSocket, which is something that can be placed into what we were just talking about and how easy it is to start looking at something and see that it has the
[42:05] issue. Even though we're like, oh, this would be really cool. And this also takes a lot of time to go through all of them. But also this is another thing that I don't necessarily
[42:18] realize that a tool changed. So I can, I don't know, let's share my own OBS or my own StreamYard really quick and look and see if it does what you're thinking about. Graham, share. Okay,
[42:37] we're going to have inception for a moment. So you can, like it used to be, hopefully you can deal with this for a moment. If you see right below here, or like towards the
[42:51] bottom above the mute stop cam buttons, that menu, there's our three images or whoever's on the stream. And then above that, I am going to make Graham go away for a second. It has
[43:03] the like different visuals that you can go to and these layouts. This has not always been here. This is something that is, I don't know when it came out, but like enough that
[43:18] something worked and I didn't go look at it better. So I can do a new layout and add items. But I think that it can only do one media slot at a time. Yes. Okay. So right. So yes,
[43:35] we have the limitation. One of the tricks that I use with OBS, and in fact, if I'd thought ahead, I could have had this lined up so I could have showed you, but trying to do it
[43:44] now live stream is going to be a nightmare, is I use an online captioning service. So like, it's just basically speech to text. I have it positioned on one of my monitors
[43:55] and then I capture just two lines of the text and I put that at the bottom of my image so that I basically have what I'm saying, showing us text on the screen. That's something called
[44:07] open captions, which basically means they're burnt into the video. Like they're part of the video itself. That's one really neat, quick, dirty trick to get it to work. Um,
[44:19] that most people can do. Unfortunately, I think you might be limited there that you can't do that one. A better way is to have actual captions, but yes, that can be difficult
[44:29] and hard work to set up. Todd did send me a link to a service that he uses that apparently will put true captions on screen, something called closed captions, which are ones that
[44:40] I can activate or switch off. Those are real captions at that point. Um, so those are the better ones, but open captions are also decent. Um,
[44:50] Um, I just want to call this out really quick too, because as you're saying where it can be on the screen at the same time, we can share screens differently. And I think that's
[45:02] a great call out and a tool that you're talking about. If, if it can do it live, like I'm using the Twitch chat just as an example is you can put, if there is something that can
[45:14] do it, um, it can show up here and you can like pop out a window to have it show up at the same time. Um, yeah. So there's, uh, this, I feel like I, we ended up going tangents.
[45:29] Hey, I said we were going to do tangents, but this, this is the beauty. It's the thing is that these things only really take one time to set up. And then once you've got them
[45:39] set up, you can use them forever and you can change the experience for somebody accessing your stream, um, in a very positive way. So if there is a simple way that we could do
[45:50] it, why not? Cause like you said, one of the big barriers and it's not, it's not as bad as it sounds to say it is, well, that's complicated. You know, now some people who are in accessibility
[46:01] advocacy would say that's no excuse, but unfortunately that is how we are as human beings. You know, if something seems insurmountable and difficult, then it's not going to get done. If there
[46:12] are other options there that are easier things that have this better impact for us. So it's on, I think it's on the companies to make it easier to do live captioning on streams.
[46:24] Obviously now that you're aware of captioning, hopefully, and we can do it in DMS after we can work out a way where you can have those on your stream. Cause that would be an amazing
[46:32] addition, um, that would really level it up. And I think not just for people who are hard of hearing and deaf, I think everybody would benefit for like me when I'm talking quickly
[46:43] and English is a secondary language, they can see what I'm saying on the screen and it helps those people as well understand what's being said.
[46:51] I agree with that. I, I have a follow up question and this is something that comes to using a text to speech a lot. I use it quite often with my dyslexia. I get really mad at things
[47:05] that don't use that very well. Um, also with setting up new tools and this is something that I think I would love to hear people's ideas for of the cognitive load to try to
[47:23] set something like this up. Like I've spent gobs amount of hours doing it and like had asked different people for help, which is amazing. A lot of it is where how to work
[47:36] through, and this might be really simple, but, um, how to work through when it's, even if you're following the directions, it's not working the way it's supposed to. I know that
[47:48] sounds very weird, but like that is something that in my own limitation, like we talked about design tools on a phone. If a menu is not working properly and I need to get to
[47:59] that spot on a site and I'm like, this is not working. It is literally an issue with the website. I personally get like, so it's like one of the few things that get me angry
[48:11] is tech, which is weird cause I'm in tech. Um, but it like it, like I literally get so fuming because I'm like, why is this not working the way it's supposed to be working? And this
[48:21] is such a big barrier that I get very stuck in, can't move past it. And it, it feels like those are types of things that show up for me that I'm curious if all of you have suggestions
[48:38] on how to work through that, because that's not something that I want to have as my own personal barrier, but I think others probably get the same way where it's like, how?
[48:54] So first of all, if someone makes things difficult for you through their poor decisions, then vote with your feet if you are able to, is the first answer there. So if it's literally
[49:06] a website and it's crap, find another website that offers the same thing. Now I know that's not always an option, but if that's, that's option one, like walk away from the people
[49:15] who don't give a crap about user experience, find someone who does. That is essentially what people with disabilities do all the time. They go onto a website, it's not accessible.
[49:25] They'll find a competitor. So nice parallel there. Second one is if you're getting to a point where you're, if I've understood you correctly, like you're stuck because you can't
[49:36] find the information you're looking for more than anything. It's like, you know, you should be able to get to it, but you can't find it. The easiest way is to try and find another
[49:48] way to source that information by either asking in public or chat GPT now is actually a very reasonable option to get. Yeah. You know, we have to bring it up at least once in every
[50:01] stream. Um, find an alternative way to get the information you need to get you past your barrier. Cause a lot of times your barrier is a tiny little part of a very, very large
[50:10] item, but that little barrier can be enough to just stop you dead in your tracks for days and days and be very disheartening. Um, but honestly, the best way is to ask people, you
[50:21] know, if you get stuck on something and you've, you know, you've put in the work, it's not you being lazy, like, Oh, I can't find it. Cause you spent 10 seconds. Like you've tried
[50:29] to find that information, ask someone who knows better go, Hey, I've really been stuck on this. And that's the only way to get past it. The only other thing I say is walk away
[50:39] and come back a day later. The amount of times that fixes me getting stressed out, stuck on something. And then when I walk away and come back and go, Oh, it's there. How did
[50:47] I miss that? It's cause you're too in it at the moment that I find that happens with me. I don't know if that answered the question to some points. I think it is just like our
[50:59] own individual. Like we all need to work through that ourselves and something of also remembering to go back to it. And that's a big reason that I, I really liked the way that you mentioned
[51:12] it when we talked about this earlier of accessibility is your overall focus. So even if you go on different tangents or rabbit holes or like squirrel, it is something that you go back
[51:24] to that is your focus. And those are overall tools and things that I pay a lot of attention to because to me, accessibility goes into also a lot of, um, neuro divergences that
[51:43] is that I personally struggle with. And, um, like being dyslexic for so long and not knowing I was dyslexic, I had so many teachers and people tell me that I was stupid when I just
[52:01] don't explain it the same way or couldn't put it together or my word structure is, uh, how to say this. Um, I forget a lot of words. Like I will try to, I have to explain around
[52:17] the word and even when I try to have a conversation with someone and I'm looking at them, this is going to make me tear up, but hey, it's a good conversation to have. It's, it's where
[52:33] people don't always realize that I'm having these difficulties. I don't make jokes of them, but I work this hard on it because other people don't have that access or support and
[52:44] I don't want anybody else to, to feel dumb or not like that they can have access. And I think it's so important for these conversations because like I couldn't imagine not meeting
[52:57] all of these people, but there's so many people that we can't, that don't have access and this is just talking. Wow. I really super crying. That's awesome. Um, first I think
[53:07] this is my first teach and text cry. Yay. Um, that means, that means it's a good stream, but, but it's, it's so, this is the point. This is the people don't realize how constant
[53:22] little things add up over time and how, you know, like, like you said, like people thinking you're stupid just cause you have dyslexia. So reading becomes more difficult. Writing
[53:33] becomes more difficult. Doesn't mean you're stupid at all. It just means that's a particular area or be quite a small area in some ways, a large area, another that you find difficult.
[53:44] But there, there's so many things that in the world that we don't see, you know, like, like you said, nobody's probably aware of the struggle that you go through because you
[53:57] do a very good job of masking, um, that particular thing and we shouldn't have to mask stuff. That's the whole thing. But unfortunately we're not quite as evolved as a society as
[54:09] we think we're still quite, um, cave mannish, cave womanish, you know, thinking in a lot of ways. And so we have a lot of situations where people get upset because you know, people
[54:23] have made dumb assumptions and I keep using the word dumb and then I shouldn't use the word dumb because that's got a negative connotation, but bad assumptions about people based on
[54:35] their own ignorance towards things. And I don't mean ignorance in the malicious intent. I mean, it's, you don't know this stuff. So you, you inadvertently say things that you
[54:50] don't understand the impact they're having. Like the teacher story is not the first time I've heard that it's quite horrendous that you started that sentence. I already knew
[55:00] where it was going and I was already getting annoyed and upset for you because that's a common thing. It's like, Oh, you struggle to read and write. You must be dumb. No, no.
[55:12] It's something that, um, and thank you everyone for your support. I appreciate it. It's also something that shows up at work. And one of the biggest reasons I left a company that
[55:22] Renee and I both worked at, um, it's, it's something that shows up so deeply and a big reason that I have my other show shit you don't want to talk about because these, these
[55:36] are so important and so integrated together that I, I now have to update Roy. Um, so Roy anger is somebody that y'all should just know about in this dope human, um, is helping me
[55:50] rebuild my website for the, I think fourth time. Um, and I've been doing it on the background and he's been helping me like figure out tags and like categories and things like that.
[56:01] And he's like, do you think teach you on tech and shit you don't want to talk about will ever overlap? Like, Oh, no, no.
[56:12] But they do in this instance, that's why the it's the so closely related and it's the, the, the, the worst part of this for me, other than obviously seeing you get upset by it
[56:25] is that we can't have those conversations. So I love the shit. You don't want to talk about that. You I'd never come across until you told me about it earlier. Uh, cause I
[56:36] love that because these are conversations we need to have and there's, it's so important to have them because the biggest accessibility barrier I think in the whole world, isn't
[56:47] like developers not using semantic HTML and everything else. It's ignorance to the fact that they should be, like I say, I keep using the word ignorance,
[56:55] but it's like, if you don't know it, you don't know it. And like bootcamps don't teach it and things like that. And so if you don't know what people are experiencing, then you
[57:07] can never have any empathy and you can never do anything about it. And the problem is it's all brushed under the carpet and nobody wants to talk about it. And I love the fact that
[57:16] you shared that with everybody here. Um, even if it was hard and difficult, um, because without people realizing what impact that stuff has, they'll make the same mistakes.
[57:30] There are probably plenty of people in the world who, because someone, you know, can't read or write all of a sudden they're like, you must be stupid. And you know what? Couldn't
[57:38] be further than the truth. Because more often than not, people who are dyslexic have a very, I don't know whether they're related or whether it's a, an adjustment or what that's happened,
[57:49] but most people who are dyslexic become very creative. I've seen that. And I know you shouldn't make an assumption, you know, it sounds like the bloody stupid superpower bollocks, but
[57:58] it's very, very true. And it has no impact in your ability to do the things that are important. It just means that if I'm aware of it, I know not to send you a massive, long,
[58:12] very thick paragraph document. I now know to send you things that are broken down sentence by sentence.
[58:18] So that's easier to not have follow up, uh, run on and, you know, make sure that I make it very obvious that you can ask me questions if something wasn't clear, or I'll send you
[58:27] voice notes if those are preferable by being able to talk about it. It means that we can work a solution out. The problem is people are so scared to talk about it because then
[58:38] there's a negative connotation and we need to get rid of that. To me, that's the biggest thing.
[58:44] I agree and thank you. It's, it's something that I will say I am so grateful for the company I work for at and the team I have right now, because like when they found out that I was
[58:57] dyslexic, they don't have me do like blog reviews, like for content reviews. Because even though I can use text to speech, it's just going to take me forever and a day longer
[59:07] or something that I think a lot of people in general that we all think a little different and learning how to work with that and talk about it, uh, as you said, um, with the, uh,
[59:22] how you could be sending somebody like, uh, voice messages or when we, um, people now ask me when they're going to be posting something, they're like, Jen, how hard is this for you?
[59:33] To read this. So that way they have an idea when other people go to read it. And I'm like, it might sound weird, but if you put a lot of emojis, like when you're trying to do bullet
[59:41] points, I at least know that we're in different areas because then it's a different emoji for each area. That's also why I probably emoji way too much. Um, and, um, it's, it's
[59:53] definitely something that having like, it's, it's, and I'm grateful that, uh, that James joined today, but it's crazy to think how he knew me back then and how I thought I was
[60:08] like the worst thing in the entire world ever. And it's, it's wanting to make sure that other people don't experience this. And Renee, I love that you found our community. Like, I'm
[60:20] so grateful that you're here and that you show up and that you hang out with us. Like it's, it's definitely something that these are all conversations to be had. And Todd,
[60:30] I'm going to bring yours up so I can read it. Um, developers do not realize the extent and portion of developer community who are disabled. And a small part of that is ignorance.
[60:42] Uh, but, uh, it's pure ignorance usually from certain communities that are toxic. And I, I do like, um, the way you say that it's, it's a big reason. And wow, I really did not
[60:57] know that these would overlap so much. Um, that I like shit you don't want to talk about is I created that show was a lot of times it's like, we're taught how to think about
[61:11] things and don't always have access or know to exist or how to ask the questions. So if you talk to people that are, um, different, like, how do you ask them about it in a way
[61:24] that's curious and not, uh, berating, but also how do you have these conversations with people that are okay with taking on the intellectual, intellectual and emotional burden? Like, it's
[61:39] not fair to be walking up to, um, like I have an insane amount of curiosity, um, and asking people like if they have an amputation, I, I have caught myself in the past that I'm
[61:57] just purely curious. It's not always appropriate to ask y'all it matters on the relationship. There's so many things that they like it's yes and no and wrong. And yes, that I like
[62:06] to do what I call bus Chuck and ask those questions on the show for us. So there's an episode that talks about like generational trauma and what that looks like, or being
[62:19] a, um, a specific race in a different parts of the U S and different identities. And all of that goes into accessibility too. So when we're talking about ignorance, it's also generational
[62:35] and it's so much harder to break apart. And yeah, I had no idea that these would tie together that much. Thanks, Graham.
[62:41] No problem. No problem. Just so you have a minute to sort of, you know, recenter and everything because like, so I could tell that was a difficult thing to say out loud. Um,
[62:51] there's something that you said in there, which is the hardest thing around accessibility is how do you ask and where is the onus on you for self-education versus the onus on
[63:02] someone who I'm going to say has a different experience in life because maybe they're an amputee where's the onus on them to explain how best to interact? For example, do I put
[63:14] my hand out, shake your hand? If you've had your right arm amputated, is that bad manners or would you consider it bad manners? If I didn't put my hand out and this is the really
[63:24] difficult conversation that you can't have. And it's the problem is we're getting worse at it, not better because social media has made us all very scared of saying, you know,
[63:36] for example, I kept using the word dumb before and I always try to self-correct because I know the negative connotation, but that fear for a lot of people will stop them having
[63:46] the conversation in the first place because they're like, what if I say the wrong word? That's the crux of half the problem though, because if you don't know what the impact
[63:56] of what you're doing, then you're never going to do anything about it. So we need to get rid of some of that fear. So I love the podcasts that you're doing. Like I said, I've never
[64:04] caught it, but I'm certainly going to listen to it now because they are important conversations and they need to be had in a frank way so that you can ask the stupid questions. You
[64:17] can ask the question that, you know, you don't know the answer to. Oh, this is the one here. I'll tell you this one. This was the one that I got right, but I really was not comfortable
[64:27] at the point that I got it right. And I don't know if it's right as a general rule. I met someone who had a hook for a hand at a networking event. And so I literally put my hand out
[64:40] and shook their hook. But in my head, in that moment, it seemed like an eternity of me asking now, is it appropriate for me to grab that hook? Is that hook an extension of them or
[64:50] is it an assistive aid that they prefer? I don't touch. Is it going to be weird when I grab the hook? Is it dangerous for me to grab the hook? It looks quite sharp. Maybe
[64:58] it's going to pinch back. All of that was running through my head. Whereas literally if someone has said to me, Hey, this is my hook. Feel free to grab it. Don't worry. It's
[65:07] like my hand. I'd have gone boom, I'm okay. I'm comfortable because we don't want to upset anyone with them worried. And I'd say my rule of thumb now has been, I asked the dumb question
[65:19] and if I offend someone, I'll apologize rather than making an assumption because the assumption is more dangerous position to be in. And so that's been my attitude.
[65:32] I also like the way that you mentioned that they could have mentioned it, but it's not necessarily on them either. To that point you made though, is it something that somebody
[65:45] needs to address themselves to share the information or something that we need to learn to ask? And that is so much, so deep in this conversation and it, I'm going to go, I'm going to like
[65:59] wrap this all, all the way back. I'll say one last thing. One last thing y'all. It's going to be great. Maybe I will. I don't know. Add to stage. There we go. Look, it has a
[66:15] link tree and I haven't, Wesley Faulkner was one of the last people I had on the show talking about intersectionality. He's big in the tech field. That's why I mentioned him. But I haven't
[66:30] had an episode since almost a year ago. So that's why nobody really knows about it. And I'm currently looking for, you know, if anybody wants to talk about this shit and wants to
[66:43] be on the show, please let me know. Because other than today with Graham, normally I don't talk about this stuff on live streams. They're pre-recorded because you know, people aren't
[66:52] always comfortable talking about it that way. Okay. Now that that's out of the way, because I told Graham I was going to bring it up and you know, I found an awkward way of doing
[67:00] it. Not awkward at all. Honestly, it's one of the, I'm going to use the word nicest. It's not the word I want to use, but I can't think it's one of the nicest thing to see
[67:11] someone just finally say the shit that they want to say. You know, it's the thing that's been hiding under the surface and no one wants to talk about it for fear of someone, I don't
[67:22] know, judging and just you sharing that today was, it is one of the things that I, I enjoy seeing that. And I don't mean that, you know, I enjoy seeing you upset. I enjoy you sharing
[67:35] that with people so that people can see, because this is the thing that, this is why I like accessibility. It's the, the impact you can have without even thinking about it. Like
[67:44] you said, the voice note thing is the simplest thing in the world, but without knowing to ask that it's very difficult to get that in place for somebody. Which is why I try and
[67:57] approach it the other way, which is I will ask someone if they're okay with voice notes, because on the flip side, someone may not be okay with voice notes at all. You don't
[68:06] know if they're hard of hearing or if they find that hard to comprehend. So asking the question, the problem is I've not got good at asking the other way, which is, would you
[68:13] prefer to have a voice note? So after today, I'm going to try and make that a thing that as I'm DMing people, I'll say, would you prefer a voice note? It's a very small change that
[68:25] potentially could have a big impact. And I think if we had more of that, sorry, I've gone off on a tangent and I'm going to go on the tangent. So I'm going to back up a
[68:34] little bit. I think in the workplace, we need to be able to, without any fear of reprisal or rejection, be able to say, Hey, I have this disability and this is what I need in
[68:46] order to do my job. I think that would be the biggest accessibility win we could have in the world. Because now that I know that you're dyslexic, immediately I go, right,
[68:59] well, what do you need? And that's the only question I need to ask. And you tell me how best to give you information. If we can get to that, that would be amazing. The problem
[69:10] is there's still the stigma, there's still the ignorance in society that we can't deal with. But that's my aim is to make more employers aware that if you ask the question, you'll
[69:22] find the people who are going to work hard for you, because you've said it yourself, you love the company you're at now. And a very brutal truth behind this that yet again,
[69:34] shit, we don't want to talk about. Here's one that will get me cancelled by saying this. But it's, you will be a more loyal employee to that company than most people who don't
[69:44] have a disability. Because you found somewhere where people have taken the consideration and the time and you've been in the position where you don't, you've had the shit experience.
[69:56] And that's a horrible thing to say out loud is one of those unspoken truths. But hell, retaining staff is one of the biggest companies, problems companies have. And if by just making
[70:08] minor adjustments to the workflow, I retain you for a year longer than somebody else. Fucking win win for me as a company, you know, and I know that's a horrible truth, but we
[70:19] could go on a whole nother tangent. I'm sorry, I'm trying to get you away from the upset bit. I'm sorry, I'm trying to. I'm good. And I appreciate that. And it's also something
[70:30] that just to mention, if people feel comfortable talking about certain aspects of their personality or their learning or things like that, it does make it easier for people to communicate
[70:46] with them. Yet not everyone is at that place or safe enough to have those conversations like physically and emotionally safe enough. And I do want to call that out because I can't,
[70:58] I do have the privilege to say, yo, I am super ADHD dyslexic. I also am bipolar type to have a dash of anxiety, depression, and a shit ton of PTSD. It's super fun. Look at the podcast
[71:15] if you want to find out more. But being able to say that to people and tell them, yo, I will probably forget to reply to you. It might be a year before I reply to you again. I don't
[71:28] mean to. We'll be friends for life. And also if I do reply to you and you may get 20 messages, like a stage five clinger in between him, because I was actually me remembering to tell
[71:39] you things. So I'm like, like one or one or the other and never know. And being able to talk about that out loud has lets people have those expectations so they know ahead of time.
[71:54] But it's taken me a lot to get here and that's why I want to bring it up. I also want to bring up the fact that, um, I don't know if Kat is still here, but Jasmine is Katnip and
[72:09] I am Sam, or I don't know what their, um, handle is off the top of my head is Kat. They, they just joined my, our discord group and they have the backwards names. So it's going
[72:25] to be very interesting to keep track of that. Um, but to bring it all the way back, what are your top five things when building a website for accessibility that you take into consideration?
[72:43] Top five. So top five things. Uh, first things first, keyboard navigation. So it's so hard to just
[72:51] randomly go back into that, you know? Um, yeah, so keyboard navigation, I will always be conscious of how will I navigate this type of the keyboard? Is this something that's
[73:04] interactive? If so, can I focus on it? Uh, centered with that, there's also focus indicators. That's one of the big ones. Have I remembered to style my focus indicators? Cause default
[73:14] ones are pretty naff. Um, so I always make sure that there's decent contrast on them. Second one, am I using semantic HTML that we were talking about earlier? Um, am I using
[73:25] something that is descriptive of what this element does on a page? So like I said, please everybody, if you ever find yourself writing a href equals hash or a href equals JavaScript
[73:37] void, you probably need a button. That's, that's my big pet peeve. Please just use buttons when you need to use buttons. That's what they're there for.
[73:46] Um, third thing I'll be thinking about and it starts early on in the thought is if I'm designing a component for a page, I will be thinking early on about, like I said, the
[73:59] keyboard accessibility, but also how is the information structured in a logical way? Is there a sufficient size tap target for people who are using either a mobile device or maybe
[74:10] have a dexterity issues so they can't be accurate. So our tap target's large enough and things like that. So those things together, all I think cover five. I don't know how many I've
[74:22] done there. Four maybe? You put, well, you said keyboard nav and focus indicators. Would that be one or two different
[74:30] things? We'll call that one because without the focus indicators, it's impossible to navigate by
[74:34] keyboard. So we'll call that one. Let's make this hard. Two is semantic HTML.
[74:40] Yeah, that's definitely one. And then, uh, three is, uh, is the component that is being built have a large enough touch
[74:50] area? Yeah. Tap target is the word I use for it. It's, it's basically, you've got to think
[74:57] of it like this, which is if someone has something like a cerebral palsy, which is a prime example of Parkinson's disease, their ability to tap a very specific point on a phone is, is it's
[75:08] very, very difficult. It requires a lot of concentration, tensing the muscles open, even then they are likely to miss. So having large tap targets, which is basically the clickable
[75:18] area is a huge win for accessibility for everybody else. It just means that you don't accidentally click the wrong link. It's a win-win, but
[75:25] you know, it's, it's less frustrating. So that's a big one that I always think about is how can I make this item, this area larger to click on that? That's a huge accessibility
[75:35] win. Uh, fourth one I'll be thinking about then is probably, I'm just trying to think how
[75:40] I would go through the process. Cause it's so automatic and I don't, don't manually think about it. I think the fourth thing that I'll be thinking about when designing the page
[75:49] is consistency because it's never a single page application. There's not, and I don't mean single page like spot. I mean, there's never one page of content really. There's
[75:59] several pages. So have I got consistent designs throughout the site? So are all the buttons similar or at least have similar styling so I can identify a button easily on the page?
[76:11] Is the navigation consistent across the website or does it suddenly change on different pages? Cause that's terrible experience for some people. So I'll be thinking about consistency
[76:21] a lot. You know, if I display images, ideally I want to be displaying them in a similar way all the way through the site so that they don't start going to random layouts, which
[76:30] can be very confusing and off putting. And then the final one I think about is language. There you go. I've thought of a good fifth
[76:37] one that isn't an obvious one. Um, reading age of a 12 year old. This is one of the rules that doesn't get spoken a lot. Um, when people are talking about accessibility, but I will
[76:50] run my reading through and I'll share this in the chat through, uh, Hemingway, the Hemingway app. And what this app does is it analyzes your writing and it gives you a rough idea
[77:01] of the reading age of whatever you've written. And it's a fantastic way when I finally get back to Twitch, it's fantastic way of making your language simpler and easier to understand.
[77:15] Um, and this is the one that shocked me the most when I got started getting into accessibility, which is in the UK, at least one in five adults in the UK have a reading age of a 12 year
[77:27] old that is expected of a 12 year old. When you consider that you realize how many people you can exclude by using complicated language. And then it's a really good one to be able
[77:40] to translate over to a business because you can go, well, one in five people are going to struggle to understand your message. If you use all that jargon, convoluted language
[77:49] and everything else, keep your language simple and to the point, stop trying to sound smart. Then you maximize the amount of people you can reach. So I love that as a fifth point
[77:58] and I don't talk about that one often enough. I hope that, I hope that fulfills the bill now Jen. Have I got five or do you need more? No, I mean, we could always have more, but
[78:08] I think five, this is a great way for someone to start. And I think in my opinion, the color contrast, those types of things would go into the consistency of design as well. But to
[78:23] read the top five, we have keyboard navigation and focus indicators. Number two is semantic HTML. Three is the component that is being, is the component that is being built have
[78:38] a large enough tap target. Four, consistency and design. And five, simple language. I'm reasonably happy with that because that covers a lot of things. You know, that's,
[78:51] those are broad things to think about where you can then go and focus on detail afterwards. The one thing I would say, if anyone here is brand new to accessibility, the first item
[79:02] I mentioned is the easiest one to test yourself on your own website without any accessibility knowledge. You can literally just press the tab key and see if A, you can get to everything
[79:14] and B, can you see where the focus is on the page? The amount of websites that fail that and web apps that fail that is astounding. So that's one to go and try yourself. If it,
[79:24] if at any point you get lost on a page or something that should be focusable, doesn't get focused when you're tapping around the page, you've got an accessibility problem.
[79:33] You may not know how to fix it yet, but at least, you know, there's an issue and you can start exploring. So that's why I love the tab test. It's, it's such a good easy
[79:42] way for people to go, oh crap, there's something wrong. I don't know what yet. Thank you. Thank you. And hello, Aaron. I think Alex brought up a, a, a great question
[79:57] of, I don't even know how to say it. Numeron? Yeah. So numeronym. So it's a brilliant thing. So you know how, I don't know if you've ever
[80:11] seen, but accessibility is often displayed as A double one Y. Yes, which Ben told me why. And I got really excited because there's 11 letters.
[80:23] Exactly. There's 11 letters in the middle. That's a new meron in right. The problem with it is it's not very accessible, is it? So it's like the, the, the irony of inaccessibility.
[80:34] We use a double one Y all the time is hilarious to me because you don't know what that word means until someone explains it to you. It's like, um, you see them everywhere in tech,
[80:46] you know, I one, a 10 for internationalization. Right. It's straight up. Um, I, um, Jasmine, I was about to put yours up and I was like,
[80:55] what is that? And then Todd put both of them up there. And I'm like. I love it. I didn't even look to the chat, but you literally picked up all the ones I
[81:04] was thinking of right there. You were. Uh, what's, what's TIL? Dude, I don't know what any of these are.
[81:11] You see, you see, that's the, that's the funny thing. So the other thing that Todd said was abbreviations. TIL is today. I learned, but until you know that, then you don't learn
[81:19] what TIL means. It's like the funniest thing ever. Um, I, I, and I realized that even if I like can pick up context, if somebody is saying
[81:29] it a lot of times, I don't remember them like, uh, goats. Greatest of all time.
[81:36] Yeah. And I was like, yo, my friend was like, Christine is a goat. Yeah. That's the thing you can get from the, you can get from the context that it's a positive
[81:49] thing, but you don't know what exactly it is. Yeah. I get that. There's a very good point there in the abbreviations thing, which is because we're
[82:01] in tech. So we are the abbreviations capital of the world in tech, like everything's an abbreviation. And so here's a really good tip for people who may write, which is,
[82:12] first time you use an abbreviation, put the full explanation of it in brackets. Just the first time you use it in each article, each page, it's a great way to make things
[82:22] more accessible because then I go onto a page, I might be new to tech, or maybe I'm new to the subject area. And all of a sudden you're like, okay, HTML, what the hell's an HTML?
[82:33] If you say hypertext markup language next to it, and then I have maybe even a link to go and read about it. I can understand what that abbreviation is for. So there's a really
[82:42] good tip. Exactly like that. Okay. Just to make sure that we had a reference, I wanted to make sure if I got it right. Yeah. Only the first time. Then for the rest of that
[82:51] conversation, you can use LOL. Yeah. I love this. This is just turning into an abbreviations game now. Is this what YAML actually means, y'all? I believe so. What does YAML actually mean?
[83:05] I believe so. I believe that's the actual... If not, then I've been fooled this whole time because that's what I thought it stood for as well. So I've either bought into a meme
[83:14] or that's the actual name of it. And Todd put... Thank you. Web accessibility guidelines. Yes. This is something that if y'all... And this is something that I... I'm repeating myself because
[83:30] I got excited. This is why we have Teach Gen Tech. Yes, I love learning and it's super fun, but it's to ask these questions. I've literally asked someone on a stream, "What is a div tag?"
[83:44] Because I didn't know. Yeah. Well, this is it. I still struggle. Yeah. This is... Oh, my favorite one there is pepcat. That's one. That's brilliant, that one.
[83:54] So that's for a way to describe people who are basically... They say something's wrong with an application, but actually it's them that's wrong. It's problem exists between computer and keyboard.
[84:09] That's what it stands for. So it's like the problem is not the actual thing, it's the person using it is the problem. Oh, and I like that. Sometimes it's just
[84:22] helpful to know the history of it. So A11Y, as Ally, also came out of earlier Twitter, they believe. So it was to minimize the number of characters consumed from the 140 character limit.
[84:40] It was never meant to really be an all-encompassing abbreviation. And wait, there's more. What is this? I don't know.
[84:54] I'm not clicking them anymore. If you're going to put them, do tell me what they mean afterwards. Oh, yeah. RTFM was the one that I thought it was.
[85:06] That's read the effing manual. So yes, I like that one. Yeah. Oh, dear. But yeah, this is the whole point. So the thing is that if you put the full expanded
[85:23] version in brackets afterwards, at least within the context of that document, even if you forgot it tomorrow, you'd understand what it meant for the rest of that article or document probably.
[85:31] Or at least you could reference back to it. So that's why I always say abbreviations are a nightmare. Expand them fully the first time you use them in any article or document or anything
[85:41] you're creating, and you make things so much more accessible pretty much for free. And also, since y'all are the community that shows up often, also, please put them in the
[85:52] chat when you're using something if it's not said on screen. So that way we know what they're talking about. Wait, wait. Wizzywig is pronounced Wussywig. I never knew that. I always say Wizzywig.
[86:05] I say Wizzywig. Oh, you see, I'm learning so much. This has been such an educational stream, Jen. I say Wizzywig. Yeah. Like what Ben wrote.
[86:17] Here's the one that... Wizzywig. Wizzywig. I've never... Aaron, do you really... I don't know if that's
[86:24] ever come up in one of our conversations. I love this. The one that I want everyone to take on board as the correct pronunciation now is,
[86:36] you know, SQL. I'm afraid it has to be said as Squirrel. I saw that once, and now I'm like, you know what? That's it. That's what it is. My Squirrel.
[86:47] Nope. Nope. Can't do it. You say it, but you... So disappointed, Jen. I wanted to do My Squirrel.
[86:56] Oh. Aaron, I can just like... Can I make you a mod or something? Hold on. How do I do this, y'all? I don't know. Oh, there we go. Oh, you can fast mod people now.
[87:08] Oh, well, that's fun. Oh. Well, a lot of it has to do with at GoDaddy, they used MySQL with PHP, my admin for WordPress things,
[87:26] and I heard it as MySQL. It is how I... It's... Stubbornly about that one. And that is also something that I... If it doesn't hurt anybody that I'm learning to just let it go. If other
[87:46] people do it differently. This is one of them, because I'm like, no, it's MySQL. If we're going to start a war over this, we have to ask, how do you pronounce this next one? G-I-F.
[87:59] How do you pronounce that one? As in the image format for animating. GIF. That's the right answer,
[88:08] as far as I'm concerned. GIF. But we will start a war now, because people will say it's GIF.
[88:15] I agree with that. I also... Just one thing that frustrated me at the very beginning was Veet. Because it's French. And so it's said as Veet, V-E-E-T, not Veit, which is how it's spelled.
[88:37] And learning the history is something that helps understand. Brilliant idea for a video. Brilliant idea for a video is, this is the correct pronunciation
[88:50] of all the things. And then you just go through all of the tech terms. Is it Versel or Versel? You know, like someone needs to, you know, we need to decide these things.
[89:01] Can we have Ellie and do it? Because I can't get their name right. They were on the screen. Okay. I don't... I must admit this. One of my very, very, very, very, very, very dear friends.
[89:19] I've been friends with her for like eight years. Okay. That is how she spells her name. And I couldn't stop saying Ines, no matter how she said it, no matter how many times she said it.
[89:37] And then all of a sudden, in March or April this year, like we've been friends for this long, I finally got that it's Ines.
[89:49] Yep. Yeah. I can see that. It just couldn't click. It just couldn't click. And I'm like, I would try, but it wouldn't click.
[89:59] So, you know, you got to do what you got to do. I can feel you on that one. We've gone so far off tangent, haven't we? It's brilliant.
[90:13] We got the five. We did get the five before we went through all of this. And thanks Todd, you brought it up. So therefore we had to like figure out what all of these
[90:21] meant. It was a very wonderful tangent. And I think a great way to, you know, sign off this stream on because it's on such a happy moment.
[90:31] Is there anything that you wanted to cover today specifically, other than us getting to the top five suggestions to think about when building a website?
[90:43] No, there's only really one thing, which is, look, some people will shout you down when you're trying to do things accessibly, especially if you say, hey, I've made this more accessible.
[90:55] There's a very small percentage of people who are going to say, yeah, but you forgot this and everything. Don't be put off by those people. Most of the community who care about accessibility
[91:04] will support you. So just try and do one thing. Like I said, go do the tab test on your own website. If you're new to accessibility and you're watching the stream, I don't know if anybody is,
[91:16] or if everybody here is accessibility focused, but if you knew, go do the tab test that I said, just try and tap around your website. And if you find the problem, then go and ask the question,
[91:26] how do I fix this? I know I have a problem, but I don't know how to fix it. My DMS are open for anything that isn't Googleable. So basically, if you, if you are trying to do something with
[91:37] accessibility, you've Googled it, you still can't find an answer. My DMS are open. I will always try and help. And I always say that very important fact that if it's something that you can Google,
[91:48] you may get a snarky comment back with here's the link to Google for the question you asked, you know, so not often. I'm just a bit spicy that way. I say still ask because specifically,
[92:02] there are a lot of things that are Googleable, but if you ask anybody that knows me well, I am the worst at Googling anything possible. Like, I don't know, like I cannot Google the
[92:15] things I literally will walk up to people and be like, this is what I'm trying to look for. How do I Google it is something that I ask people often.
[92:22] So in that case, special, special exception for you, Jen, because we know each other. No, just, just say that. So I'm horrible. Like a big part of it, y'all is if you're asking for help,
[92:34] tell people what you've looked for, tell people the work you've done. Because even though I may be horrible at Googling things, if people understand that they're like, oh, well, that's
[92:45] cool. Well, try this instead. Um, and it's very important differential because yes, as Graham said, a lot of people will try to reach out and they haven't said anything. And it is like,
[92:59] yo, I'm not going to do your homework for you. So Todd has kindly said that anyone can DM in and he won't be a prima donna like me.
[93:08] Look, I get so many DMS now on Twitter. I just can't handle it when people say hi. So that's, that's where it comes from. It's not meant to be hostile, everybody. I want to be clear.
[93:19] It's just, I get so many random hellos that I just, I've grown tired. I've grown tired of it. Anyone on the stream is welcome to DM me whatever they want. How's that? Are we happy now?
[93:30] Is that less hostile? No, I like this. I like the spicy take. I did like the spicy take. And, um, I, I also,
[93:39] I find it really funny. I feel like I shouldn't say this, but I feel like somehow either Twitter really protects me from it or people just don't reach out to me on Twitter that much.
[93:51] Like people just, I don't have the random DMS. Even, uh, when Jasmine and I started talking, like we DMs like a while ago from, I think a Twitter space, like, I don't, I don't know.
[94:06] I think I meet everybody through Twitter or streams or stuff, but as some of you are in this, but if you're not, uh, you can join our discord group because we're cool. And, uh, my D and D
[94:21] friends, um, have been pushing me to actually talk about our community and have a place where people can go because they're like, Hey, we have the Oatsman Source Raid group, uh, discord.
[94:35] So you should, um, have people join it and talk to you about your shows. And I was like, Oh, I should probably do that. So now I'm actually doing that. And some of you are in it already,
[94:48] which is awesome. So, yeah. So, um, Todd, we're not doing D and D at the moment right now. Um, we're, we stopped our last campaign, at least that I was playing, um, that I was a part of in,
[95:03] I don't know, way earlier this year. So, um, Oh yes, Alex, uh, Todd, you can do a one-shot on the expanse. It would be really cool. We need to tell you about Roy. Roy is the game master and
[95:19] the one helping me build my site. And these are also a big, like a big reason I really like this community is I go, Hey, I'm trying to do something. Is this even possible? Or what do I Google? And
[95:33] it's a great community to do that because they're all way smarter than I am when it comes to all this tech stuff I've been learning. And they're very wonderful at teaching and frustrating me
[95:46] to learn myself, but helpful. That's what you need. And also, look, I've put it off on a tangent here as always, it seems to be my superpower, but, um, ask the questions, even if you think
[95:59] they're dumb, like we said that earlier, um, but find the place where you feel comfortable to ask those questions that you're like, I should know the answer to that. I've had to lately ask lots
[96:09] of questions that you would think someone who's been a software developer 15 years would know, which are things like, Hey, how do I get react app to work? Like the fact I'm asking that question
[96:19] to most people would be shocking, but I never play with it. So go and ask them questions. Better to ask the questions and learn than to sit in ignorance all the time. So I'm sorry. I said
[96:29] about the DM thing, just DM me, ignore me. It's fine. Uh, but go find the place where you can ask the questions. And I agree with everything you were saying there, Jen, like you have to be able
[96:39] to go and ask the questions and get the answers in a way that works for you. I think that's a better answer than I give originally. We have, and we're happy with that one, I think.
[96:49] I will. Okay. Now you're going to, I'm going to go on a tangent now, you have to protect your bubble. You have to protect your bubble. Like if you don't protect
[96:58] your energy and your bubble and things going on, people will just take, take, take, take, take. And the way you phrase things, I liked that it's a way of, of doing that. And also like,
[97:13] you're going to have people like me that are like, but what about this? Which is really annoying. Like I annoy myself about this stuff. I just want to let you know,
[97:23] like it is, it is awfully annoying, but it's something that it's all a balance and finding your own guidance. And a big reason that I think Graham's hilarious and super fun is learning
[97:35] to just be who you are, no matter who that is and your people, you'll find your people. Yeah. I always go by a rule of a third of people in the world will like you. A third of the people
[97:49] will tolerate you and a third of the people won't like you. And you know what, there's seven and a bit billion people. So two and a bit billion's enough to go out for me. I'm happy enough with
[97:57] that. You know, I like it. I like it. All right, y'all. Uh, I'm going to see if anybody's online. Oh, Chris is online to raid too. So we'll raid to him. Amazing. And we will see all of you later
[98:15] and I will be back next week. Actually, Roy and Jacob are going to be on here next week about clerk. We're going to learn about authentication. Yeah. Yeah. And I'm, I have so many questions for
[98:30] them. It's going to be exciting. So see you sometime on Tuesday. Cause I'm not great at being consistent on timeframes just on Tuesday. That's what we're going to stick with Tuesday-ish.
[98:41] And bye y'all. See everybody. Thanks for having me, Jen. Yeah. Bye. [BLANK_AUDIO]

