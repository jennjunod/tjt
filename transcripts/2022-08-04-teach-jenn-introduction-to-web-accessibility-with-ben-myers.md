---
showLink: "https://www.youtube.com/watch?v=OPzr8vDNZ9Y"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-introduction-to-web-accessibility-with-ben-myers"
title: "Teach Jenn Introduction to Web Accessibility with Ben Myers"
publishDate: "2022-08-04"
coverImage: "https://i.ytimg.com/vi/OPzr8vDNZ9Y/maxresdefault.jpg"
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
[00:06] We have Ben here today, and we're going to learn lots of fun stuff.
[00:12] Please introduce yourself and what we're going to be learning about today.
[00:15] >> Howdy, howdy all. It is great to be here. My name is Ben.
[00:20] By day, I'm a software developer at Microsoft working on their documentation site.
[00:25] But where folks probably know me around is that I'm a web accessibility advocate.
[00:31] That's what we're going to be talking about today. But I've blogged about accessibility at benmeyers.dev,
[00:36] and I actually host a stream of my own called Some Antics, where every week I bring on a guest from
[00:42] around web development and web design to teach me something about building great user experiences for
[00:46] the web in a hands-on way with a focus on accessibility and core web technologies.
[00:51] Jen, do you think I need any more caffeine? >> I'm still like I have my rock star in the background,
[00:59] so I have water. I'm thinking about caffeine too.
[01:03] >> I have caffeinated water right here. >> That's a thing?
[01:07] >> Yeah. It's like flavor packets that you can mix into your water,
[01:10] like fruit flavored packets that have caffeine in them. I don't know. I dig it.
[01:15] >> All right. I didn't even realize that was a thing. >> I came here on the stream and I'm
[01:19] already feeling so attacked right now, Jen. >> What? You're teaching me all the new things already.
[01:24] >> Exactly. There we go. Anyways, we're going to be talking about web accessibility.
[01:31] Before I get too much into what we're doing today, I wanted to actually get a feeler from you,
[01:37] Jen, as to what is your understanding of web accessibility and what it entails?
[01:43] There are no wrong answers here. I just want to see where you're at just to start.
[01:48] >> I appreciate that and I love this is something that I really appreciate when guests do this,
[01:54] just in general, checking and understanding of where someone's at before explaining it,
[02:00] because then it also helps someone course-correct or add to their understanding.
[02:07] Thank you, first off, for asking. I would say if I, let's see.
[02:12] When I think about web accessibility, I think of, we talked a bit about screen readers,
[02:20] which we will go into a bit more about that. You explain it so much more,
[02:24] not the same as text-to-speech, which I learned. The reason I mentioned that is
[02:32] text-to-speech does not or something that is not accessible, is if you put a PDF or a PNG or a photo of a graphic,
[02:47] that is not something that's accessible to a screen reader or excuse me, a text-to-speech.
[02:54] They can't read a PNG a lot of times. Then also colors.
[03:03] >> Okay. What have you heard about colors, Jen? >> What up Brazil?
[03:09] >> Hey Brazil, good to have you. >> That not everyone can see all of the colors,
[03:15] so there are web accessible colors, but also being able to invert the colors.
[03:22] >> Okay. Interesting. Good to see where that's at.
[03:27] Accessibility, this is one of the hard things, and actually one of the things that I should give as
[03:33] a caveat before we get too deep into this, which is that web accessibility is a massive umbrella,
[03:41] and there's no way I can teach you everything you need to know about accessibility in an hour.
[03:45] There's no way I could teach you everything you need to know about
[03:48] accessibility in a day, in a week. It's a continual learning process.
[03:52] Today, my goal is not to make you an accessibility expert. My goal is to just provide an entryway,
[04:01] get you start to think like an accessibility practitioner, and hopefully get you to
[04:08] the point where you could start to discover more. >> Captions.
[04:12] >> That's another one. Yes, absolutely. >> I might randomly be yelling these out the entire time.
[04:19] >> Web accessibility, broadly, I would define as usability for disabled users.
[04:30] We are making sure our site is usable by disabled users. If you think about the words,
[04:39] disabled users seem so simple, but that is a plethora of people.
[04:45] That is a diversity of experiences because disabilities come in all shapes and forms.
[04:51] There are many kinds of disabilities that all have their own needs.
[04:53] Two people with similar disabilities could still have entirely different needs.
[04:57] Also, one of the things I think often gets left out when we talk about disability,
[05:02] is that if you have one disability, surprise, you actually usually have at least three.
[05:08] There's this intersection of different disabilities, so if we're talking about
[05:13] this theoretical disabled person, there's only so much of
[05:19] people's experience we can capture with that. As part of this,
[05:25] what I'd like to do is just spend some time. This is going to sound a little ridiculous,
[05:29] but I'd love to just spend some time, Jen, if you could just name some disabilities you know of.
[05:34] Just as many as you can think of. >> Another one that came to mind,
[05:41] and this goes to naming a disability of blindness, and there's different degrees of blindness.
[05:49] That reminded me of another one, which is increase in font size,
[05:55] or different font styles, and boldness as other accessibility options.
[06:02] Deaf, not being able to use the screen itself, mattering if that's because of hands or something,
[06:12] like not being able to use the screen itself, or a website itself.
[06:19] I feel like on the spot that I'm blaming all of them. >> By the way, folks in the chat,
[06:30] if you want to comment, just some of the various disabilities you know of.
[06:35] Again, I know this exercise seems a little ridiculous, but just name as many as you know of.
[06:40] But it can be hard to think of these things on the spot. One thing that might help is that many accessible.
[06:48] Yes, absolutely, Rizal, spina bifida, yes. >> What is spina bifida?
[06:54] >> That is wonderful. I'm pulling up Wikipedia because I'm not going to do it justice.
[07:00] Let's see here. What is spina bifida? It is a birth defect of where there is
[07:05] an incomplete closing of the spine and the membranes around the spinal cord during early development and pregnancy.
[07:13] Yes, it is a disability of the spine. Got you. Rizal's husband's twin brother has that,
[07:29] so it affects his walking. Absolutely. Many accessibility practitioners will,
[07:35] just to help us start to think about disability in a way that we can start to incorporate into our work,
[07:43] they'll categorize different kinds of disabilities. There's your vision disabilities.
[07:47] You mentioned blindness. There's also low vision,
[07:50] which is a degree of blindness. But a low vision user might have different needs than a blind user,
[07:57] so we might also separate those. There's also colorblindness, etc.
[08:03] Colorblindness is especially prevalent in men. I want to say like eight percent of men,
[08:11] like one in every 12 men, has some form of colorblindness,
[08:16] most commonly red-green colorblindness. Colorblindness is something to consider there.
[08:22] There's hearing impairments. We've talked about that a bit.
[08:24] I myself am hard of hearing, so I can relate.
[08:29] You've got your mobility disabilities, things like Spina Bifida,
[08:35] but also more links. Awesome. >> I just posted it because it's
[08:42] the disability and health overview from the CDC. But I like the way you're explaining it,
[08:48] so I don't want to go over to that. I just really wanted to make sure we had the link.
[08:53] >> You're totally good. Mobility disorders could
[08:56] be something like limb deformities, like I've got. You could have, for instance, Parkinson's.
[09:03] You could have arthritis. There's so many things,
[09:09] and what those are ultimately going to do is probably impact your ability to do things with precision.
[09:15] It might be hard. You might not have the fine motor abilities to be able to
[09:20] move your mouse exactly where it needs to be, for instance. Then there's a whole host of cognitive disabilities as well.
[09:27] We could talk about, there's ADHD, there's autism, there's short-term memory loss,
[09:33] there's dyslexia, dyscalculia. There's so many.
[09:37] We could spend all day naming a bunch of disabilities. But broadly speaking, this is a diversity of experiences,
[09:44] and everyone with those disabilities is going to have some impact on their ability to navigate the web.
[09:51] Our goal as web accessibility practitioners, you and I, Jen, is to ensure that
[09:58] those people still have equitable access to their sites. This could be something as seemingly unimportant as
[10:09] being able to order a pizza online to something all the way as critical as managing your finances.
[10:16] I used to work at a bank, and one of the things we were taught is that elders,
[10:24] as they old, old is officially a verb apparently, as they age, as a result of
[10:32] both physical and mental disabilities that they could get while aging,
[10:36] they aren't always able to manage their finances independently. They oftentimes have to have a younger family member
[10:44] or a loved one deal with their finances for them. This actually puts them at
[10:49] significant risk of being taken advantage of. Elder fraud, elder abuse is
[10:53] absolutely a common thing that banks have to worry about. But if a website were designed such that
[11:02] our grandmothers could manage their finances independently, that puts them in a situation where
[11:09] they're less likely to get taken advantage of. This is a direct tangible way in which
[11:14] accessibility seriously matters for real people. >> There is a lot to take in there,
[11:22] and I love how you mentioned also physical disabilities. We talked about the blindness or hearing or those type of things,
[11:37] but also the invisible ones like dyslexia, and ADHD.
[11:46] It's weird because those are things I'm very passionate about, yet I sometimes forget that they are also disabilities,
[11:54] yet because the term neurodiversity is used instead. It's so true that they are because there
[12:05] are a lot of things that I need help with on websites. I was talking earlier about the text-to-speech.
[12:14] I don't know, maybe I'm going to be using a screen reader after this.
[12:17] I really appreciate you going through all of those and sharing those experiences because the list that the website says is vision,
[12:27] movement, thinking, remembering, learning, communicating, hearing, mental health, and social relationships.
[12:36] Everything you just mentioned falls into that. I learn a lot easier by somebody talking to me
[12:44] about it than reading off of a website. I think that is so cool having these type of
[12:50] conversations because it's different avenues of learning as well. >> Absolutely. Ultimately, the hardest part of
[12:59] accessibility is the empathy part because I'm disabled, you're disabled, we have disabilities,
[13:08] but we don't have all of them. We don't have universal disability experiences
[13:12] because there's no such thing. Ultimately, as web accessibility practitioners,
[13:17] anyone who's doing web accessibility is going to have to try to find a way to put themselves in other people's shoes.
[13:24] They're going to encounter the web in ways in which you and I don't on a day-to-day basis,
[13:32] and still have to figure out what is a meaningful experience. I've also put another link in the Twitch chat.
[13:39] Backing up here, all of the specs that are standard for the web are put together by
[13:49] an organization called the World Wide Web Consortium. They have a sub-organization called
[13:54] the Web Accessibility Initiative or WAI. I've shared a link to a resource from them.
[14:01] This w3.org/WAI/roles/users. Wow, and what this is,
[14:10] is, oh, is that the one I was thinking? There was, hang on.
[14:17] I think they've changed things. >> There's an introduction to web accessibility here too
[14:23] that I think would be very helpful. >> Here's the page I was looking for.
[14:27] I'm sorry. I've just put in the Twitch chat. It's this people-use-web.
[14:33] Then what this does, is this goes through basically personas of people with different disabilities,
[14:41] and talks through how their disabilities impact their web experience.
[14:46] For instance, because I'm hard of hearing, things like listening to podcasts online,
[14:53] or watching videos online, can be difficult unless there are captions or transcripts.
[14:59] So this page is a good way. We won't be going through this today,
[15:03] but this is a great place to just get an overview for how might disability intersect with people's experience of the web.
[15:13] >> I love this. >> Yeah. This is absolutely worth giving a read.
[15:19] >> One thing that I think is, I'm wondering how when you talked about it,
[15:27] that it overlaps is like, I believe you mentioned about languages,
[15:33] and being able to make that accessible as well. Would that go into web accessibility,
[15:40] or would that be a different area altogether? >> This is an interesting question.
[15:46] This is something I think folks in accessibility spaces can sometimes disagree with each other on.
[15:54] You'll have some people, for instance, that will slot in things like performance into web accessibility.
[16:00] Because if your site is slow and takes forever, then you significantly disadvantage people
[16:08] from areas with lower socioeconomic status. So folks will make the case that performance enables access,
[16:17] therefore performance is accessibility. I tend to focus specifically,
[16:22] I think performance and internationalization and the like, these things are very important.
[16:27] I prefer to focus web accessibility as a category on disability in particular. However, I think there are still a lot of intersections
[16:37] between performance and accessibility, and accessibility and internationalization.
[16:42] Folks will disagree with me on that, but yeah. >> I'm curious if that changes based on the target audience of the website.
[16:55] For example, if we're talking about having to work on any government documentation, like let's say getting one that comes to mind and is close to my heart of immigrants.
[17:10] If they're unable to read the government websites because they don't speak English,
[17:16] I'm like, "Okay, cool. Yeah, that's probably something that it may fall into accessibility."
[17:20] Whereas if we're talking about APIs, maybe not something that's as important.
[17:30] I don't know. That's just what came to my mind. I can see it being debated either way,
[17:35] but that's a conversation for another day. >> Yeah. This is probably what we're doing.
[17:44] For the purposes of today, we're defining accessibility as specifically around usability for disabled people,
[17:51] which has a lot of intersections with other parts of the web. There are many reasons to care about web accessibility.
[18:00] I like to think of it in terms of what anchors developers to accessibility rather than what are the motivations.
[18:11] My anchors are that it's personal for me because I'm disabled. I believe that access is a fundamental right.
[18:22] I believe it's a civil right. I believe that this is the right thing to do.
[18:28] I also, in my experience, have found that accessible sites usually require
[18:34] a stronger foundation of our HTML and stuff like that, in such a way that it actually makes our site more robust for a lot of
[18:41] other things that we might care about like performance, or internationalization, or a search engine optimization.
[18:47] Accessibility is a vehicle to get to other things our businesses care about as well. Stuff like that. Also, I work in the front end.
[18:58] Usability is the job, I feel. If you're a front-end developer,
[19:04] your job is fundamentally to create a usable experience. Whether you're doing that with some framework like React,
[19:13] or whether you're doing that with just plain HTML, or whether you have whatever back-end, does not matter.
[19:21] Your user doesn't care. Your business partners don't even care.
[19:25] The only people who care are developers. Because at the end of the day,
[19:30] the interface that comes out is what matters. That's what users see.
[19:34] They don't care what tools you've used for this. They don't care that you've slung around some JavaScript in a cool way.
[19:38] They care about whether they can use it. Usability is fundamentally your job.
[19:44] I don't know of any front-end developer who wouldn't be at least somewhat bummed if they found out that someone couldn't use their site for some reason.
[19:55] Usability is the job. There are other anchors that people have.
[20:02] Some people will point to something called a curb cut effect, which is in disability academia,
[20:08] it's the notion that accommodations for disabled people can indirectly benefit
[20:13] non-disabled people as well in ways that you don't expect. Closed captions are a prime example.
[20:18] Therefore, people who are hard of hearing or deaf, or have auditory processing disorders,
[20:24] but they also benefit people who are in the bar. There's a sports game that they want to watch,
[20:30] but they're in a bar, it's loud. Other people will point to lawsuits.
[20:36] There are lawsuit websites, like businesses have gotten sued because their websites are inaccessible.
[20:44] Folks will point to that as an anchor. Stuff like that. There's tons of things that could anchor you to accessibility.
[20:52] I would encourage anyone who's interested to start to think about why they care. I can't give you that answer,
[20:59] but those are some of the reasons I care about. >> Thank you for sharing that.
[21:05] This may be a question for another day, but I would love to have you on the show again to
[21:11] also specifically talk about accessibility for developers. Because that's a big reason why an anchor for me of
[21:22] starting Teach Gen Tech is showing people that tech is accessible for everyone. It's not something that is just if you can afford a boot camp or something like that.
[21:36] I would love to have that conversation with you later. I know we don't have the time today.
[21:41] >> A point I'll make is that right now, in some ways, tech is not accessible for everyone.
[21:48] Because a lot of our resources are like video courses that don't have captions and stuff like that,
[21:54] or blogs where the images don't have alt text and stuff like that. Tech could be accessible to everyone.
[22:00] But in the context of disability in this case, it isn't always.
[22:05] I think considering accessibility within the industry is very good. Wow, it is amazing how time flies though.
[22:18] Do you want to look at a website? >> Yes.
[22:21] >> I built ahead of time. I should give the caveat first of all,
[22:29] that I did not totally build this. I actually found a template from a site called html.design,
[22:35] and then I adapted it to make it inaccessible. I'll share a link to,
[22:39] you're looking at the hosted version right now, and I'll share a link to if anyone wants
[22:44] the GitHub repo because we are going to be messing with the code a bit today, I'll share a link to that as well.
[22:49] Let me just get that first. I've put these links in the Twitch chat.
[22:56] My goal here is I've put together, this is a very plausible seeming modern day website
[23:04] that's riddled with inaccessibility issues. Today, we're going to just spend some time putting
[23:11] ourselves in the shoes of various disabled people, figure out where they might have some problems,
[23:15] and see if there's ways that we can fix them in some cases, or at least talk about at
[23:20] a high level what we could do to fix some of these things. At first, I think we should just do some exploration phase.
[23:27] I think we should just look around the site. If you're finding something where in your mind you're like,
[23:34] "Hang on, a person with such and such disability is already going to struggle with this," just call it out.
[23:39] I want to just know your free and open thoughts about the site. >> For sure. What up, Anthony?
[23:48] Thank you for joining, as you can. To recap, because looking at the chat totally distracted me,
[24:00] call these out as we're exploring or wait for [inaudible] >> Just look around and if you're like,
[24:07] "Hey, I can think of," and if it would help, we can also just straight up maybe come up with
[24:12] a few disabilities that we could try to specifically put ourselves in the shoes of.
[24:18] But yeah, just look around the site and see if you can identify anything that you think would be an access problem to someone.
[24:26] >> I've already blown up this page quite a bit, and this text is still incredibly hard to read.
[24:37] >> It is, isn't it? >> It's something that a lot of the text can be hard to read.
[24:43] I also know this because on my podcast website, I really like this cursive,
[24:48] and I always have to think about that. I can't overuse it because it's not accessible,
[24:53] and it can be very hard to read. Is there a way to see if,
[25:04] I don't know if it's SEO or if it's accessibility, but I feel like there's a way that you can
[25:17] put text as an explanation of an image. Am I just making this up?
[25:23] >> Yeah. What you're describing is something called alternative text or alt text for short.
[25:29] There is an accessibility requirement, and you should put a pin in that,
[25:34] that I just mentioned the word requirement, you should put a pin in that.
[25:37] But there's an accessibility requirement that any non-text content that isn't decorative needs to be described with some alternative.
[25:50] So for images, when we've got the image tag, the angle brackets IMG,
[25:56] there's an attribute that you can add called alt. In there, you put a description of the image,
[26:05] and the goal of that is that you describe basically what someone's saying. You convey this to, for instance,
[26:17] people who use screen readers. A screen reader user could navigate to that image with their screen reader,
[26:24] and they would be told whatever the contents of that alt text are. There's tons of blog posts out there of like,
[26:34] "Oh, how do you write good meaningful alt text?" For me, it boils down to one heuristic,
[26:39] which is that I like to imagine that I'm on the phone chatting with a friend, and I want to tell them about this cool image I have in front of me.
[26:50] That's how I like to think about it. That's what keeps me like making sure I'm providing
[26:56] enough detail that it's meaningful without going overboard. Because you can start to do things like,
[27:04] well, if I'm talking to a person, a friend, and maybe the image I've got in front of me is a picture of President Joe Biden.
[27:14] I could just say it's a picture of President Biden. Maybe describe what he's wearing, what he's doing.
[27:19] But it's President Biden. I don't have to say a white man with white hair wearing a suit. I could say President Biden because people know who that is.
[27:29] The whole imagine I'm on a phone call thing is a heuristic I've found is really helpful for me at least.
[27:38] You've called out that like, "Hey, we don't know yet,
[27:43] but it seems like maybe this image isn't being described with alt text." Or at least you wouldn't put it past me to have not described this image with alt text.
[27:53] >> Okay. I have so many follow-up questions later on. Ben, I'm hoping to volunteer you,
[28:03] you'll have to come back because there's just so much on this. I don't know about the images.
[28:15] >> Yeah. Because this is a scaffolded site, we're going to see tons of placeholder images.
[28:20] >> Yeah. >> That's not part of it.
[28:23] It's just I didn't have time to go find a picture of strawberry. >> Yeah. I think the alt text also shows up here.
[28:29] But I think the part that I was just stuck on is I don't know if the vegetarian part is going to be readable here to let somebody know
[28:40] if that is something that would be able to be screen-read. >> As a general rule,
[28:51] text on the page is able to be screen-read. Now, whether it's meaningfully associated with
[28:56] the other contents is a different story, right? >> Got it.
[29:00] >> Folks using a screen reader in particular would be able to get to the word veg or non-veg.
[29:05] >> Got it. Okay. Cool. >> There's caveats and stuff like that,
[29:10] and your information architecture needs to be good. But broadly speaking, that won't be an issue.
[29:17] >> Okay. I don't think I am seeing really. Other than colors.
[29:28] >> Tell me more. >> If you're colorblind,
[29:33] you're not going to be able to differentiate very well with the reds. I believe reds are not a color that is color accessible.
[29:45] Do I remember correctly? >> This is interesting.
[29:49] First of all, what we're describing here is something called color contrast. The idea here is that we have some text on a background,
[30:00] and that text needs to stand out from the background for it to be readable. Typically, what we would need to do is we would want to compare
[30:11] the color of the text to the color of its background. In the case of this nav bar that we've got,
[30:18] where it says Home, Recipes, Restaurants, we would want to compare the white of the words,
[30:24] the white of the text with this red background. Do you want to do that?
[30:29] >> Sure. >> Here's what we're going to do is,
[30:33] can you right-click on one of those links and then do inspect element? Inspect, yeah, there we go.
[30:41] Then over in the very bottom right, you can see that the color of the nav link is pure white, FFFFFF.
[30:52] >> Yeah. >> It's pure white. That's going to be easy to remember.
[30:57] Then in the elements pane to the left, if you scroll up a bit,
[31:01] there's going to be, I want to say it's the div class equals container, is what has the red.
[31:09] No, I'm sorry, it's the header class equals header. That's what it is. Now, if you go to the right,
[31:15] there's this background color EA3C53. Let's copy and paste,
[31:21] or let's copy that hex code there. >> I'm done.
[31:28] >> All right. Now, we're going to go to Google and we're going to search for color contrast checker.
[31:34] There's tons of these out there. There's one that I end up using quite a bit,
[31:38] but virtually any of them will do. That first one is the one I end up using, so let's use that.
[31:44] This is by a resource called WebAIM, which is a fantastic website to learn about web accessibility.
[31:51] >> It's five, right? >> Six. There'll be six of those.
[31:59] >> All right. Let's scroll down and let's see what we're finding here. First of all, that sure is a lot of acronyms in gobbledygook.
[32:10] You've got this number thing. What's the deal with this number?
[32:15] First of all, I guess, what is your first question when you're seeing this?
[32:24] What is the first question that comes to mind? >> Question would be, yes,
[32:33] I'm curious what the aspect ratio is, but just taking a look at this,
[32:36] I like how it automatically gave us something that would be a pass. It doesn't make me have to think about it very much.
[32:45] It makes me go, "Oh, okay, cool." The graphical objects and user interface components,
[32:53] I'm like, that would be the easiest and not a ton of thought process going into it. But the normal versus large text,
[33:02] I'm like, "Oh, yeah, that totally makes sense."
[33:06] But the contrast ratio, the biggest thing is what's the best score?
[33:13] >> Yeah. Let's talk about this. As for your question of what's the best score,
[33:18] contrast ratios are on a scale of one-to-one to 21-to-one. One-to-one is you've compared a color against itself.
[33:27] There is no contrast because it's literally the same color. Then the max is 21-to-one,
[33:34] and there's only one color combination that can give you that. Do you want to take a guess what that would be?
[33:39] >> Black and white? >> That's correct.
[33:42] >> Yay. >> What we can see here is that it is this exponential thing.
[33:53] Once you start getting more contrast, you get more and more contrast faster.
[33:57] A lot of the colors that we tend to see in the web tend to fall in this three, four-ish range, probably a little lower as well.
[34:05] But let's talk about these pass and fail tests. First of all, there is this WCAG,
[34:15] and that stands for Web Content Accessibility Guidelines. Those are the guidelines, those are the requirements.
[34:21] I mentioned earlier that we should put a pin in the fact that there are accessibility requirements.
[34:26] Those accessibility requirements are the Web Content Accessibility Guidelines or WCAG.
[34:30] They have different standards for different kinds of content when it comes to contrast.
[34:38] WCAG has three tiers of strictness. There's level A, which is like,
[34:45] you've maybe thought about accessibility before. There's double A, which is the industry standard.
[34:51] Then there's triple A, which is like, wow, you're super compatible with all the things.
[34:56] Double A is usually what we target. It's the industry standard,
[35:00] it's the legal standard if you're thinking about this in terms of compliance and not getting sued.
[35:05] With that in mind, what we're looking at here is, we care about all the lines that say WCAG AA,
[35:12] because AAA is usually not within reason for us. It's the pie in the sky.
[35:21] Ideally, you could make this, but most people don't try.
[35:25] With that in mind, for a large text, for a large text, we're passing.
[35:35] Large text, there's a whole definition of it, but basically, it's either big or bold is what it translates to.
[35:41] You could read the explanation, but because there's a specific combination there,
[35:46] but bigger bold. But in large text,
[35:50] needs to meet a ratio of three to one. Well, we're almost four to one.
[35:54] We're doing pretty good if this were a large text, if this were like a heading, but it's not.
[35:59] It's a normal size link. Normal text, which we can see we're failing,
[36:04] needs to meet 4.5 to one. Anyways, so yeah, that is.
[36:16] >> We have. We've been bumping up the fonts. It's been fun.
[36:21] >> There we go. Yeah, there we go. I wrote a blog post actually about color contrast,
[36:27] that I'm going to link in the Twitch chat. If you're not here on the Twitch side, you're missing out.
[36:34] But yes, I wrote a blog post on the subject. Folks who want to, absolutely should check out.
[36:43] But as it stands, our color for the size of our text doesn't work.
[36:50] We go back to our little demo site here, and we look at that nav bar again.
[36:59] We have two ways we could fix this. Do you want to take a guess what those two ways are?
[37:06] >> We could make it bold or larger text. But the suggested way from the web contrast checker
[37:16] was to make it have a white bar behind it and black text. That way, it has the highest contrast.
[37:25] >> You don't need to have the white and black. You don't need to do that.
[37:32] What you could instead do probably is pick a darker red. There was a tool recently I ended up using.
[37:41] Let's see. I'm going to send the link in the Twitch chat, but I'm also going to send this in
[37:53] our private StreamYard chat so you can see this. See, that works. What you've done is you've come up with
[38:00] a color that works really well for every center. You could do this. If you want,
[38:05] we could do this on our local version of the code if you want. >> I feel like this does show a pretty good explanation of it
[38:15] because then you can move these around to be able to see maybe some colors you might like or don't like,
[38:23] and then even changing to different parts. So that's the background and then going like this.
[38:33] >> Yeah. >> That's cool.
[38:34] >> I love playing around with this. The other site I've linked you to,
[38:38] let's you plug in two colors and then it'll be like, "Hey, I found the closest match basically to get the ratio you want."
[38:47] There are tools to help you pick better colors that are going to work. But broadly speaking, for this particular issue,
[38:54] we know how to fix this. We could either make the text bigger or we
[38:59] could pick a different red or a different color altogether. >> I love that. That makes sense.
[39:11] We already talked about the ones on the screen and all text. Did I miss anything?
[39:20] >> That's a great question. You have, but that's okay. Because basically the site is
[39:29] designed as a choose your own adventure when it comes to accessibility. You figure out a few things that are interesting and of note,
[39:37] and we follow that trail. Part of the thing is you're not going to be able to see,
[39:45] literally visually see everything that's wrong with the site. But maybe let's follow one of these links.
[39:53] They're all going to take you to the same dummy recipe page, because there's only one of those on the site.
[40:00] But now we have a new page. Maybe we spend some time on this page just looking around seeing what there is.
[40:09] >> It doesn't look like this had auto captions burned into it, but you can turn them on.
[40:16] >> Yeah, absolutely. Anthony's right. I just used that tool yesterday to fix something on his podcast site.
[40:25] Sorry, the contrast finder one. With captions, there's this notion of open captions versus closed captions,
[40:35] where open captions are the ones that are burned into the pixels of the video itself, and closed captions are the ones that you could toggle on and off.
[40:42] I personally, in my experience as a deaf person, I prefer closed captions.
[40:49] They usually let me change how the captions look. If the captions are wrong or if they're in the way, I can turn them on and off.
[40:58] I personally prefer closed captions. There's nuance as to when you might want to use open captions, but yeah.
[41:07] The fact is there are at least automated closed captions on this video. I wouldn't necessarily flag that as a problem.
[41:16] >> Cool. I did want to turn it to a part just to see if they had it with open captions. Let's see. What else?
[41:28] I can make the text even bigger. Well, the colors again.
[41:39] >> Yeah, we know how to fix that for sure. >> This is still small, so not exactly the same, but pretty similar.
[41:50] >> Those grays are pretty light, aren't they? >> Yes.
[41:55] >> We could conjecture, and I'll go ahead and confirm, but we could conjecture that those grays don't pass color contrast requirements either.
[42:03] >> Interesting. Do people get paid to go through websites to check accessibility? >> Yeah, there are services. I know one service is called Tenon.io.
[42:16] It's run by an accessibility practitioner named Carl Groves. He's a contractor that you could hire out basically to do an audit of your site.
[42:24] There are services that'll do that, yeah. >> That is cool.
[42:28] >> Anthony's right. Yeah, and they should be paid way more. Yeah, in general, there's a lot of times you'll see companies that don't value
[42:39] accessibility expertise will try to find a way to get that expertise for free, which is absolutely a sickening plague on the accessibility community is companies
[42:51] that don't value accessibility work, but just want the free labor basically. Yeah. But I'll tell you how I really feel. But anyways, yeah, let's keep going.
[43:03] >> All right. Anthony did just comment, "Accessibility is so technically challenging and incredibly important, and no one values it enough." I already had some ideas of this
[43:24] beforehand, and now just talking today, I'm just like, "It's even more." I would say in general, this text is hard to read.
[43:35] >> It is, isn't it? Fun fact, I did not change anything about that text from the template I grabbed this from. >> Is that why this doesn't look like
[43:48] Arial or Times New Roman? It looks like something else. >> No, that might be Montserrat. I think that's actually Montserrat.
[43:55] >> Is there a font that is more accessible on websites than others? >> That's a great question. So I actually did a stream with a professional typographer
[44:09] named Bruno Mog. Let me see if I can find a link to this. Yeah, there are fonts that do score better on readability, basically. Hang on. Sorry. I'm doing too many things at once. But there are
[44:28] kind of attributes that lead to generally more readable fonts. So you want something that's thick enough. You also want something that has fairly even stroke width throughout, right? You don't
[44:41] want something where the vertical lines are really thick, and then the horizontal lines are really thin, or something like that. That tends to pose a readability problem. But yes, absolutely, there
[44:52] are, you know, fonts that are more or less readable overall. There we go. >> There was one that I was told about because of being dyslexic called Comic Mono. And that is
[45:10] something -- and there's plug-ins for a browser to do it. So that way -- because one thing that you mentioned earlier is they're not all -- disabilities -- different disabilities have
[45:25] different needs. So it may not be the type of thing that I would want to put an entire website in this Comic Mono. But finding some that are a bit better for it. So thank you for posting the
[45:38] video. >> Yeah, the whole subject of like dyslexia fonts is kind of a tricky one. There are fonts that will claim to be dyslexia
[45:54] friendly that maybe don't have as rigorous academic backing as you might think. However, if they work for you, you should absolutely have the choice to use them. And this is a thing that
[46:07] hits home a lot in accessibility, is that because there's a plethora of experience and you can't just make one broad statement about any disabled people or any group of disabled people, choice,
[46:21] personalization is something that matters, right? The ability to opt into a bigger font size or even a different font altogether or light mode versus dark mode or something like that. Being
[46:31] able to opt into the settings that work best for you is a huge part of accessibility. Because the thing that people get wrong about universal design is that you can and should have a one size fits
[46:47] all solution. You can't. Because everyone's different. But instead, what you can do is you can enable people with your design to pick the approaches that work best for them.
[46:57] >> That's making me rethink about how, yes, I want technology to be accessible for everyone. Yeah, you're absolutely right. It's never going to be fully accessible for everyone. But with
[47:12] these type of tools, it can make it accessible for more people. So, I really appreciated that call out earlier. We already talked about the gray. And I know I'm probably missing more,
[47:32] but I feel like those were the because these dots are really hard to see too. >> They are, aren't they? Yeah. >> And just such a small font here.
[47:44] Anyone else seeing something that I may have missed? Anthony, are you seeing anything? Because I did probably miss something. I should say, what did I miss?
[47:56] >> Oh, yeah, I can work on that, Anthony. Broadly speaking, so we're looking at a and I'm hosting this demo on Netlify. So, you can look at this same site.
[48:12] Here's the GitHub repo. We've mostly been doing just kind of a cursory like visual check. So, we've been looking at things like color contrast. So, the web and color contrast checker is kind of
[48:24] the main other tool that we've looked at. >> And I've been asking Ben to come back on again because I think realizing and seeing these is going to be like being aware of it is like the
[48:38] biggest part of like knowing the change and then hopefully Ben will come back on and like then we can go through and see how we start doing the changes. Because I think that is like a big like
[48:51] two-piece part of comprehending and then actually changing. >> Yes. Okay. So, here's what I want to do next because we've kind of looked at a few things here and there, right? But I have alluded
[49:06] a couple times to there are accessibility defects that you literally cannot see on this page, right? And so, I want to help you basically figure out like get to the point where you can
[49:19] start to discover more of these things. And so, I'm going to recommend you install a browser extension. This is called axe dev tools. That's axe as in like a lumberjack tool. And I will get
[49:31] you there's a link in the chat. But if you go to like the Chrome web store. Oh, I see. Yeah. Yeah. There we go. Yep. All right. And you're just going to click that add to Chrome button. So,
[49:49] this is by a web accessibility resource called DQ systems. DQ is phenomenal. They have a great website where they provide a lot of accessibility information. I would trust them with my life when
[50:04] it comes to accessibility stuff. And so, what axe does, this is a browser extension that will let you scan a page and it will give you a report of automatically surfaceable accessibility issues
[50:19] that won't be every issue. That can't be. Because, you know, you can't magically check everything with a computer. Yeah. So, we are going to have to yep. Yeah. There we go. And so, yeah. Let's
[50:33] go ahead and hit scan all of my page. Oh, hello. Interesting. Oh, can you restart your browser? Hopefully this isn't the browser that has Screamyard open. >> I have it open in a different
[50:51] tab. But please hold. I can do something else. Give me a second. I'm going to go back to us and then I'll change some things around. I just have no idea what I have open in my other browsers.
[51:05] Totally fair. Yeah. We just need, like, I think a new browser window. Yeah. And if you want, I can actually also do this on my end if you'd prefer.
[51:16] Yes. You can teach us and navigate. >> Let me start sharing my screen here. Just a sec. Got to allow. Okay. So, hopefully I think at this point we've now got some recursion.
[51:34] Yeah. We should do. All right. Yeah. So, I'm on the recipe site. And here's what I'm going to do is I'm going to open up my dev tools. Oh, that has opened up over here. So, I'm going to now run
[51:49] this is the same extension you've got. I'm going to click scan all of my page. And this is going to, again, come up with the automatically serviceable accessibility issues. That won't be every issue.
[52:00] But it can tell you, for instance, hey, this image is missing alt text. It can't tell you whether that alt text is good or accurate, right? So, there's still usability concerns here. But
[52:10] as you can see, let me actually rearrange this so we can see everything better. As you can see, it tells me, like, oh, on the home page, we have 44 issues. Let me maybe put these side by side.
[52:25] There we go. So, we have 44 issues that it's come up with. So, 16 of those are color contrast issues. And then there's one called, like, HTML element must have a lang attribute. Well, I wonder what
[52:42] that's about. So, if I scroll down here, it will actually give me some information of, like, oh, here's your element, right? Here's how you find this. But then if I keep looking, there will be
[52:55] this link here that says more info. I really like clicking this link. Because a lot of times I find that in accessibility, I don't know why something's a problem, right? It's, like, there might be a
[53:09] requirement for something. My automatic tool might come up with something, right? But, like, I don't know why it's an issue. Why does it matter that my HTML element must have a lang attribute, right?
[53:21] So, I click this page, and it takes me to a page that Deque has about this exact issue. And I'll send that link in the chat here. But, yeah, so, what this is, the lang attribute lets you specify
[53:37] the document language. For, you know, our purposes, we'll want lang equals EN, because this is an English language site. And then I can scroll down here, and it will tell me why it matters. And
[53:48] broadly speaking, it matters because assistive technology, like screen readers in particular, want to know how to use or, like, want to know how to parse our page, right? And so,
[54:00] they'll want to know, like, what pronunciation packs do I need to load and stuff like that. And so, I like looking at this, because this tells me a lot about, like, who needs this and
[54:12] why is this a requirement? That can give me a good sense of how to fix it, too, right? Because I might look at this and go, well, okay, I recognize that the automated tool is giving me
[54:22] this issue, but the real problem is actually something with my design, for instance, right? I could change my design instead of going specifically with the fix that's being suggested.
[54:32] Does that kind of make sense? It does. Something that's coming to mind for me is there are a lot of small businesses and things that would be open to changing these, but they're using things like
[54:47] Squarespace or Wix or those type of things, and that is something I'm going to be digging into, because I just looked at my podcast website, and just on the homepage, it has 14 errors,
[55:03] or 14 things that can be changed, or excuse me, 12, 12, yay. And I really like how it says critical, serious, moderate, and minor, and I'm curious how, with a web builder,
[55:21] what is going to allow us to change things around and be able to, you know, make it more accessible. So that is something that I'm actually going to do tomorrow, because I don't have anybody on the show,
[55:37] and it's definitely interesting that there's so many of these options, and yet I will say for myself, and I think this is something that is also changing the practices that each of us do,
[55:52] of it is really hard for me to just like get captions going and then post them on the YouTube video, and also make it accessible in text, and like a transcript or something like that. And
[56:08] something that I'm going to challenge myself to do is a video slash text of best practices to do that. So then you know I'm going to end up hitting you up to let me know if I missed stuff,
[56:24] just as something as content creators that we can be more conscious about. Absolutely. Yeah, so obviously like again, this has been such a broad introduction,
[56:39] and there's so many rabbit holes we could go down, right? We haven't, like we've maybe even just like barely just been able to scratch the surface, and so we'll definitely do more streams,
[56:49] and I can show you more things, but broadly speaking again, we're building websites for people. We're building websites that people need to use, and our job, our fundamental job,
[57:00] no matter what tooling, or structure, or frameworks, or whatever, no matter what we're using, our job is building interfaces that people can use, and that includes disabled people,
[57:11] because we do have disabled users. They're already using our sites, and so broadly speaking, every once in a while, just try to put yourself in the shoes of, you know, someone who has a
[57:23] different disability, and figure out like if I were this person, what is something that I might, that might be a barrier for me, right? And then don't just take your guesses for it, like don't
[57:36] just take your own word for it, right? See if you can seek out blog posts, and tweets from people who do have those disabilities, and see how they describe their web experience, because it's almost
[57:46] definitely different from how you'd anticipate, but yeah, look for, yes, but like look for ways to discover more. So I mentioned the web content accessibility guidelines. Those are the industry
[58:03] and legal standard for web accessibility on our site, and in fact, I will drop a link in the chat to that document, and one of the things that's just kind of fun to do every once in a while,
[58:17] if you're a nerd like me, is here we go, is just kind of scroll down this page, and find a requirement. Maybe next time we talk about like how to read WCAG. Maybe that's something that we
[58:29] do. I also wanted to get to like screen reader stuff. We didn't even get close to that, but like that's totally fine. Kind of read through this, and just be like, hey, if something surprises you,
[58:41] right, where you're like, huh, I would never have thought of that. Why is the case? Read more. See if you can figure out why it's an accessibility issue, and see what you can do to
[58:49] improve that on your own site. And thank you for that, and thank you for getting us through the first step of, you know, looking into this, and this is something that we should all look into
[59:00] early on, and thank you, everyone, for joining. What up, B1 minds? And we're about to end. >> Yeah, and I have a stand up to get to. >> Yeah, hit us up with questions. This will
[59:15] be on Twitch and on YouTube, and let us know, and we will have Ben on again. Yay! >> Woo! Looking forward to it. Bye, y'all. >> Bye!

