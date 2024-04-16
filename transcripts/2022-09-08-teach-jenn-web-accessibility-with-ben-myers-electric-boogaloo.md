---
showLink: "https://www.youtube.com/watch?v=nTKmQoU0hXg"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-web-accessibility-with-ben-myers-electric-boogaloo"
title: "Teach Jenn Web Accessibility with Ben Myers Electric Boogaloo"
publishDate: "2022-09-08"
coverImage: "https://i.ytimg.com/vi/nTKmQoU0hXg/maxresdefault.jpg"
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

[00:00] If you wanted to wait. Hello, beautiful humans. You guys can see my, I got blood work done today.
[00:06] So you guys can see that on my arm right now. That's cool. But hello, beautiful humans.
[00:11] Welcome to another stream of Teach Gen Tech, and we have a returning guest.
[00:19] >> That's me. >> Ben is back to talk about accessibility,
[00:22] which I'm excited about because it's been stuck in my head, and I get yelled at by bots.
[00:29] Ben, please introduce yourself and what you're going to teach us today.
[00:33] >> Yes. Well, first of all, I want to congratulate you on your blood in fact working.
[00:37] It's good to hear that your blood does work. Yes. Howdy, howdy. I'm Ben.
[00:42] I blog about accessibility occasionally. I stream about accessibility far more often.
[00:48] Maybe that's the world's shortest introduction to me. I host a weekly show where I bring on guests to teach me
[00:54] something about accessibility and web development and just building great user experiences for the web.
[00:59] So this is my second time on. The first time, we talked about
[01:05] accessibility very, very broadly, I feel like. We talked about, and just like minutes before the show,
[01:14] I mentioned in the green room that I'm going to have you do part of this introduction as well.
[01:17] But we talked about the wide, diverse spectrum of disability that exists,
[01:24] and we talked about just some ways in which disability can impact your experience with the web.
[01:30] It sounds like that's been stuck in your craw just a bit over the past month, right?
[01:36] >> Yes. >> I would love if you could just talk me through some of
[01:40] the takeaways you've had and some of the things you've learned and been thinking about in the vein
[01:46] of accessibility over the past month or so. >> I would say one of the biggest things is remembering to
[01:55] do alt text for images, and there's a bot on Twitter that likes to yell at
[02:03] me when I don't put it on there, which I think is really helpful because
[02:08] it's a helpful reminder to put alt text. The thing that I have found frustrating is the fact
[02:18] that you can't go back and update alt text after Twitter has been posted.
[02:27] That's really frustrating because it's not something I always think of,
[02:33] but then I'm like, "Oh, I should have done that. Whoops, and I can't go back."
[02:36] By alt text, just for that clarification for the viewers of it is, let's see if I can describe it.
[02:44] It is a text box that is associated with an image to describe an image to someone that may not be able to see it.
[02:53] >> Yeah. We'll actually get to see some effects of that today, I think. >> The other part that's been really stuck with me is contrast.
[03:05] >> Yeah? >> Don't know. That just really stuck with me about contrast and being able to,
[03:10] are these going to be good pairings? It's interesting to me because I feel like I've always been very,
[03:19] very curious about the fashion world and colors that go together or don't go together or patterns.
[03:28] It's interesting of how much that goes into the videography worlds. If for anyone about to go on a show or something,
[03:38] you don't want to wear very small squares or stripes or stuff like that, it can really mess up the way the video picks you up for the image.
[03:51] But then also, it's so much deeper than that when it's about websites. It was really stuck with me because I never realized how
[04:05] much accessibility can go into all these other avenues than just web. >> Yeah, absolutely.
[04:16] It's one of those things where conventional wisdom can be wrong. Where in web, we've seen time and time again the trend towards minimalism.
[04:31] Show as few things as possible and see if you can tuck away, hide the things that you don't think people should care about.
[04:39] But what that leads to is, oh, well, the bits we want to hide,
[04:44] maybe we'll put this in a really, really light gray so that it doesn't stand out.
[04:48] Yay, minimalism. Maybe for someone with standard visual perception abilities,
[04:57] it's still totally feasible to read that text. But for anyone with impacted vision in some way,
[05:07] you've just introduced extra barriers, extra circle there. We've got this baseline assumption,
[05:17] this default assumption of who we think is using our page, and very rarely do those assumptions actually include disability.
[05:24] >> Interesting. >> Yeah. A lot of how I see
[05:32] accessibility work is about bashing in the assumptions we make about our users. You and I, or I guess I,
[05:47] I don't want to presume too much about your vision, but I can look at something and go,
[05:51] this is plainly readable. Sure, that's a light gray, but I can plainly read it.
[05:57] But if I'm doing that, I'm not taking into account people who might have
[06:03] been colorblind from birth or might have developed cataracts. A thing I learned earlier today,
[06:10] as you age, some of the cones in your eyes become less sensitive, and this actually shifts your perception of color over time
[06:21] away from your ability to perceive reds and whatnot. >> Interesting.
[06:25] >> Yeah. We have a lot of these built-in assumptions about our users and how they navigate the web.
[06:32] Accessibility is about breaking in the door and recognizing that this isn't a hypothetical.
[06:41] We have users who experience the web differently than we do, and they have every right to experience the web and have access to the web.
[06:48] A lot of what we're going to focus on today is this concept of an assistive technology,
[06:56] which is, I would define it for the purposes of this conversation, a piece of hardware, software, or operating system level setting
[07:07] that disabled people can use to better facilitate navigating their device, navigating the web, etc.
[07:15] >> I dig it. I don't want to go in and rehash this from last episode. We did talk about a lot of different disabilities and how they may show up.
[07:28] For those watching today, I would challenge you to just be open to what we're talking about today,
[07:38] but then also be open to, is that something that would help your own life?
[07:44] Instead of going through, well, this is for this exact disability or anything like that.
[07:50] It can be so helpful in many other ways too. >> Absolutely. The first place I want to start is with keyboard navigation,
[08:03] because this is one of those things that a lot of people benefit from keyboard navigation.
[08:09] Awesome. Yes, you've got the demo I sent over. Cool. Keyboard navigation is really helpful,
[08:17] especially if, for instance, you can't use a mouse.
[08:21] That could be, for instance, people with mobility disorders such as arthritis or Parkinson's, for instance.
[08:29] People who might struggle with the precision control that a mouse might require. You think about it like a mouse cursor is,
[08:39] the cursor itself is something floating around this intangible two-dimensional plane. A mouse cursor is not a very helpful model
[08:49] for people who are blind, for instance, or have a high degree of vision impairment.
[08:56] Keyboard navigation also impacts people with visual disabilities as well. >> I think we talked about the curb cut effect last time,
[09:10] this idea that disability accommodations can benefit non-disabled people as well. If one of your hands is occupied,
[09:19] say maybe you're a parent holding your newborn, you might not have ready access to your mouse,
[09:25] and so it might just be easier to use your keyboard. Keyboard navigation is hugely impactful for power users of technology.
[09:34] You find that the better you get with computers, you tend to just be able to do things faster with the keyboard than you would with the mouse.
[09:41] Lots of people benefit from keyboard navigation. You've probably already started incorporating.
[09:46] If you're a developer or even just tangentially in this space, you probably already begun incorporating keyboard navigation techniques
[09:53] into your experience of the web. We're going to practice a few things that you can do with keyboard navigation.
[10:06] Jen, I want to start with what your baseline knowledge is. What are some keys you can use or some ways you can use your keyboard to navigate a site?
[10:15] >> The first thing that comes to mind is the search function on Mac, which is the command space by default.
[10:27] I say it that way because I don't know where half the stuff is on my computer. Without that, I would not know how to use the calculator on
[10:38] my computer or search different things. It can search my documents,
[10:43] it can bring it up online. It is something that I use on a regular basis.
[10:49] Also, another keyboard shortcut that I use on my computer is something that I set up with Snagit,
[10:56] which is able to take screenshots, and it's like if being able to do that and multitask.
[11:04] When I hear full keyboard things, it makes me start thinking of macros,
[11:12] and I don't know anything about that. I've always been like, that's cool,
[11:21] but those are ones that come to mind. I realize that I probably use you more than I realize.
[11:28] >> Sure, absolutely. We're going to talk about keyboard shortcuts that are built into the browser,
[11:32] but I wanted to circle back to the Mac feature that you were talking about, which is called Spotlight Search,
[11:38] which is when you do command space. If you think about it, that's an assistive technology.
[11:44] Jen, pardon me if I'm wrong, but you're open about having ADHD, right?
[11:50] >> Yeah, I'm ADHD, I'm dyslexic. >> I want you to consider the Spotlight Search and ADHD assistive technology.
[12:00] Because a thing that I have noticed for folks with ADHD, is having a rigid organization is not always helpful.
[12:10] You don't necessarily know where you put things, and having a directory structure where you have to specifically hunt down,
[12:17] oh, I put this file in this folder, in this folder, in this folder.
[12:22] >> Yeah, I never remember. >> Yeah. The Spotlight Search allows you to treat
[12:29] your entire file system as a doom pile, a doom drawer. >> For those listening, a doom pile or a doom drawer when associated with ADHD,
[12:42] is many individuals with ADHD really struggle with executive, what is it called?
[12:52] Executive function, I believe, where basically you might want to clean everything,
[12:58] but it doesn't necessarily make sense where you would put it, so you end up piling it all together where it's cleaned up,
[13:04] but it's a doom pile. It goes there. You don't know where else it's going to go,
[13:08] so it's just going to go there. >> Yeah, it's out of the way,
[13:11] but it's not necessarily like a neurotypical person's not going to look at this and go, "I see the Dewey Decimal System you've implemented here."
[13:18] >> Yes. >> Just all of the things in a mishmash.
[13:22] >> That is honestly how I think that is a great way of describing how my computer is set up, that is how my life is set up,
[13:31] and it's not something that I'm consciously going, "Oh, yes, let me do that because that sounds cool."
[13:37] It is honestly, and now that you mention it, I lose graphics on my computer all the time unless I just leave them in my download folder.
[13:47] If they're not in my download folder, I'm like, "I don't know what I called that or where I put it."
[13:53] >> Even before we get to keyboard navigation, this gets to something I want to emphasize,
[13:59] which is just about anything can be an assistive technology. We're not talking about necessarily things you have to
[14:07] purchase or things that have the accessibility label on it. Another thing that I want to consider in this camp
[14:14] of assistive technology is password managers, like LastPass or 1Password or anything like that.
[14:23] An upcoming standard of the Web Content Accessibility Guidelines that I think is supposed to be made official in December actually has
[14:33] an accessibility requirement for websites to not break password manager functionality. Because remembering secure passwords is what we consider a cognitive function,
[14:45] and that can be especially difficult for people with memory issues. >> I'm just laughing because I literally,
[14:53] to get into an account like Google, it locks me out and I have to reset the password.
[14:59] I've reset my passwords on almost everything so often that it is because of Google's backup security of allowing you,
[15:09] if you have it on your phone or something, that has caused me to not get completely locked out of all of my systems.
[15:16] A password manager would be phenomenal. I should actually look into that.
[15:20] >> Yeah. I don't think a password manager was built with specifically disabled people with memory issues or ADHD in mind.
[15:34] >> Right. >> It's a powerful tool for that.
[15:37] The impact that it has is a disparate impact where it benefits everyone. Seriously, if you don't have a password manager,
[15:45] get a password manager today. But it especially benefits people with cognitive disabilities in a very real way.
[15:54] Another person that it might benefit is someone who needs to use voice control. You can imagine having to announce your password aloud with voice control,
[16:05] A, is unreliable because we know how good voice control is, it's messy. B, it's insecure because if you have to do that when you're in public,
[16:13] you've just absolutely neutered the security of your password. >> I think that's another one that you mentioned about accessibility as well,
[16:24] is using voice-to-text. That is something I use all of the time and I can see how difficult.
[16:33] I know how annoying it is when it doesn't work. But being able to have to do that for your password,
[16:40] I would become livid at technology. Technology and I fight sometimes.
[16:46] >> Absolutely. Assistive technology is just anything that a disabled person needs to use or can use to better facilitate
[16:57] their ability to navigate their devices or navigate the web. Again, let's actually get to keyboard navigation.
[17:07] But I think that this has been a very valuable segue or detour, that's the word, because it really hits something home about
[17:15] just the variety of assistive technologies that are out there, and even just the perhaps necessity of creativity in what we consider assistive tech.
[17:33] >> Right. >> Yeah. In the browser,
[17:38] we have a few very standard means of navigating a page with a keyboard. The first one that I want to talk through,
[17:47] actually, I want to see if there's a way to open up in that code sandbox, if there's a way to open it up just so that you can just see the page.
[17:54] I think you see that like jklvhb.csv.app. If you just open that up in a new-
[18:05] >> Thank you. I was like, I don't know why I'm looking.
[18:07] >> Yeah. Just remove the distractions. There we go. >> Okay.
[18:12] >> This will make things easier. >> Really make things easier.
[18:14] >> Yeah. Thank you. This is just a simple form. I have done nothing special here.
[18:19] I haven't done anything to customize the keyboard experience. All of this is just baked into the browser.
[18:26] >> Cool. >> We've got a couple of links.
[18:28] The first thing I want to introduce you to is the concept of focus. Focus, we should think of as,
[18:35] it's where the keyboard cursor is. The idea here is your keyboard
[18:42] will navigate between different interactive elements, different things that, well, let's just see it.
[18:49] The way to focus is you hit the "Tab" key. Let's just hit "Tab" and you can see.
[18:54] >> Yay. I went to a hyperlink. >> You went to a hyperlink?
[18:58] Yeah. Let's just keep going. >> Yay.
[19:05] >> Okay. What do you notice about this? >> That it does do that,
[19:12] but I'm like, I don't know how to, oh, that was complicated.
[19:15] I went to developer to see if there were other job titles and I hit "Enter". >> Yeah.
[19:22] >> Because I was like, I would have to click it to see the other options, but it's actually a down option, a down button instead of.
[19:29] >> Down works. Space also works, I think. Important thing to keep in mind,
[19:35] these elements are all part of a form, and in a form context,
[19:39] "Enter" always means "Submit". >> That's fair. It's just more like one to three years.
[19:50] I don't know if "Shift+Tab" works. >> "Shift+Tab" does work.
[19:55] Yeah. "Shift+Tab" can move you backwards in the focus order. >> Then "Submit".
[20:06] >> Yeah. >> That was fun.
[20:08] >> This is the world's quickest demo, but what it hammers home is a few things.
[20:14] One, it hammers home, here's how you move the focus, it's tabbing.
[20:17] One thing I want to point out is that only certain things were tabbable, only certain things were focusable,
[20:25] and all of those things were interactive in some way. Our heading, our static text,
[20:33] even the labels for the different form fields, those weren't focusable.
[20:37] The only things that we could tab to were things that were interactive with the keyboard.
[20:43] With the hyperlinks, by the way, you could use, I want to say it's space.
[20:53] I could be very wrong. No. "Enter"? It's "Enter".
[20:56] >> I don't know. It's not opening it. >> I set the hyperlink to be basically blank,
[21:01] so it would just go to the same page. That's poor demo on my part there.
[21:09] To activate the button, if you tab down to the button,
[21:15] you could do "Enter" or "Space", I believe. >> Yeah. Broadly speaking,
[21:27] what we're doing here is we're tabbing between interactive things. When we get to something like the select drop-down for the job title,
[21:37] you're on the single element that is the select, that drop-down. To further interact with it,
[21:46] you have to use "Space" or the arrow keys to make your selection there. Then when we got down to the radio buttons,
[21:55] can you tab down to the radio buttons for me again? A thing to note is that this whole thing,
[22:02] your focus currently seems to be on the radio button that says "0-1" in this case.
[22:09] But if you think about it, the focus is bigger picture.
[22:12] It's really on this whole group of radio options. You can't tab to each of them individually.
[22:18] You're using your arrow keys right now. >> Right. Even if I go up and down,
[22:22] it's still the arrow keys. It's still only going within here instead of
[22:27] a tab or a shift tab that can go backwards. >> Yeah. That's something that one thing to point out,
[22:36] all of this stuff, if you go back to the code sandbox link, where you can actually see the code,
[22:43] I'm going to indicate something here. When we look at the HTML,
[22:48] I haven't added any JavaScript. All I've done is I added some CSS,
[22:53] but all I've done is implemented everything in good semantic HTML. Semantic HTML, or you'll sometimes hear it called semantic markup,
[23:04] is this notion that we are using elements that best describe the expected behavior,
[23:11] functionality, meaning, and stuff like that, and the browser will take care of the functionality for us.
[23:17] The fact that we implemented things as a select with options, meant that we got that drop-down behavior for free.
[23:27] The fact that we implemented input fields, and select, and radio, and stuff like that,
[23:33] that gave us all of the keyboard behavior we needed just out of the box.
[23:37] We had to do none of that. >> Very cool. Hello, Anthony.
[23:42] >> Anthony's here. Hello. >> Yay.
[23:45] >> Let me show you one more cool thing with this. Oh my God, Anthony.
[23:50] Let's go back to the little demo link for that forum, where we were just seeing just the forum.
[23:58] I want to show you one more thing, and this has nothing to do with keyboard navigability,
[24:02] but it is an accessibility feature. Can you click one of the form fields labels?
[24:08] >> No. >> What happened there?
[24:13] >> I can double-click it. Wait. An abusive or insulting.
[24:20] Sorry, I just started. >> I think you've got to like it.
[24:24] >> Yeah, it's grand really. >> But you can single-click.
[24:27] >> Yeah, you can single-click. >> I cannot single-click it.
[24:30] It only goes to the forum though. >> If you think about this,
[24:34] this is actually intended, and I can show you how this was done.
[24:38] But if you think about it, this is actually a really good thing,
[24:42] because what you've effectively done is when you click the label, the forum field that the label is connected to gets focused.
[24:49] This is really cool for, again, people with mobility issues that might struggle with precision,
[24:55] like tapping things precisely. It's also really beneficial on mobile where things show up far, far smaller.
[25:01] Effectively, what we've done is our label adds to the overall hitbox of the forum field. That's a hugely important accessibility feature.
[25:12] The way we did that, if you go back to the source code again, is the input has an ID,
[25:20] and then the label, you'll see that the ID here is name.
[25:24] What's confusing is that there's also a name attribute that's also set the name. You can ignore the name attribute,
[25:29] but this label has this four. We can see it better, I think,
[25:34] with the select because the select has the same functionality. There's that select element has an ID of job title,
[25:44] and above it, there's a label with a four set to job titles. The fact is that the four attribute matches the ID of the forum field,
[25:55] and that's what connects it to. >> Very cool.
[25:59] >> Yeah. That's keyboard navigation and a bit of other stuff besides. But yeah, do you have any questions about that?
[26:09] >> Not about what this is doing. My biggest question,
[26:14] especially because this is what the Latin thing that comes with the gibberish. But something that came to mind that is something that I really struggle with
[26:29] is the fact that if I was sent this form, I honestly would just skip the paragraph and just fill
[26:36] everything out without realizing what the form is for because it's going to take me too long to read.
[26:41] >> Sure. >> How would somebody,
[26:45] if they used some type of reader, would it still read the labels
[26:51] or because the label goes and clicks the actual bubble, or would you be able to?
[27:00] I hope you get what I'm saying or asking. >> You're asking about screen readers and actually, yes.
[27:09] Because we did that whole for thing, that's another accessibility benefit is you effectively name the field.
[27:16] When the screen reader user navigates to the field, they'll be told, "Edit text name,"
[27:23] or "Drop down job title development," or something like that. The exact announcements differ based on what screen reader,
[27:30] but you'll be told the name that you gave it because you've linked up the label element.
[27:36] >> Okay. >> Doing that whole for thing,
[27:40] that is required more or less. There's nuance there, but you basically need to do that
[27:46] for the for attribute thing to have an accessible form. >> Got it.
[27:53] >> Yeah. I think that can actually segue us into using a screen reader.
[28:03] >> I have been in the fortunate position of introducing people to screen readers many times.
[28:11] What I found is that if you don't go about this in a very specific order, people will have a very overwhelming first impression of a screen reader.
[28:28] What I'm going to do before I tell you how to even turn on your screen reader, is I'm going to tell you how to turn off your screen reader.
[28:35] I'm going to give you your panic button, your escape hatches. >> I'm laughing because I used to work at Verizon for many years,
[28:45] and it was right when the iPhones and Androids launched. When people would turn it on,
[28:51] it was hysterical that they would go all the way to the store to get it to be turned off, which believe me, it was annoying for me too,
[29:00] and it would be that overwhelmed yet it was also really funny. >> Yeah. It's very amusing,
[29:11] but it's one of those things where I've noticed people get this very sour first impression of screen readers,
[29:17] and then they don't know. They've resolved to never touch it again with a 10-foot pole.
[29:24] We're going to be using the screen reader that is built into Mac OS, and that is called VoiceOver.
[29:32] VoiceOver has two escape hatches I want you to remember. The first, if you don't want to turn off the screen reader,
[29:41] but you just want it to shut up immediately, hit "Control". >> Okay.
[29:47] >> Control should always work. Control, that's the instant shut up VoiceOver command.
[29:53] >> I dig it. >> What is the shut up VoiceOver command?
[29:57] >> Control. >> Awesome.
[29:59] >> I want control back. >> Yes, exactly.
[30:03] The other thing that you can do, if you just want to turn off VoiceOver completely,
[30:07] VoiceOver will have a little readout. It'll have this black display with white text on it that says,
[30:14] it reads out what the screen reader is reading aloud. In the top left corner,
[30:21] there's going to be a little white X. It looks like an ornamental detail.
[30:25] It doesn't look like it's a button, it's a close button. If you click it, that will turn off VoiceOver completely.
[30:31] Those are your two escape hatches. >> Thank you.
[30:35] >> One thing I've noticed when doing this over streaming is that you basically need to use those escape hatches frequently.
[30:43] Otherwise, you or I are not going to be able to hear each other. Just be very overeager with your escape hatches.
[30:50] >> Got it. >> Cool. With that in mind,
[30:52] are we ready to turn on VoiceOver? >> Nervously, yes.
[30:56] >> Okay. There's nothing to worry about. The way I do this is,
[31:02] I like to open up Spotlight Search, Command Space, and I like to type in accessibility.
[31:16] There we go. All right. Then that first option there,
[31:22] yep, and this is going to open up your accessibility settings. There are keyboard shortcuts to do all of this,
[31:28] but I find it easier to remember to go through the Spotlight Search. Again, doompiles.
[31:33] In the left-hand nav, there is an option that says VoiceOver.
[31:38] Yep, and there's a checkbox that says Enable VoiceOver. It's going to think for a bit,
[31:47] especially because it's the first time. Use VoiceOver. Yeah, go ahead.
[31:53] It will think for a bit. >> It scared me.
[31:58] >> I can't seem to hear it, but that's fine. >> It talks faster too.
[32:16] >> Yeah, it's very fast. >> Well, I think my spoken content is sped up.
[32:25] >> Okay. >> Maybe not. What would you like me to do?
[32:30] This is exciting. Is there a way to hear my voice or voice, my screens? >> Yeah. If you can do that,
[32:38] that might be helpful because I can't hear it. I don't think the viewers can hear it and I don't know when to start talking.
[32:46] I don't know when you've used your escape hatch. I don't know if StreamYard lets you share audio.
[32:53] >> I will look really quick. I see what you mean and why people want it to go away easily.
[33:03] >> Yeah. >> That was overwhelming is a very, very good way of saying it.
[33:09] I don't see a way to share audio, but hey. >> Folks at home can follow along with their own screen readers.
[33:16] But in that case then, because I don't know when it's actually
[33:20] talking versus when you've used an escape hatch, I'm going to need you to explicitly tell me.
[33:25] Basically, I want to queue up an exercise at a time, if that makes sense. >> Okay. Cool.
[33:32] >> I'm going to introduce you today to a few different ways to navigate a web page using a screen reader.
[33:39] The first one that we're going to do is just simply tapping. This is no different from when you were just tabbing for keyboard navigation.
[33:49] But this time, you'll have a screen reader just also telling you some things. All of your shortcuts,
[33:55] all of your arrow keys and space bars and enters and stuff like that, your tabs, your shift tabs,
[33:59] it's all the same, just now we have a screen reader. Let's go ahead and do that for a bit.
[34:04] >> It is definitely like it's reading it out loud. It just read that it is which
[34:28] Google Chrome profile I'm using and that I'm in a text box. >> Yeah.
[34:34] >> To display a list of options, press "Control Option Space".
[34:49] >> I'm glad that I can see this at the same time because it is very confusing. At least, if I were just listening without the context of this,
[35:22] but I feel like if it were somebody that maybe a bit more experienced with not being able to see it,
[35:30] that they would be able to get used to the way it's describing something. >> Yes. Real day-to-day users of screen readers will have
[35:39] this much faster than you or I might when testing. That's a thing to call out.
[35:45] You just get more used to this and you can better discern what's being said. Additionally, some folks aren't hearing their screen reader aloud,
[35:54] but rather they're using a peripheral called a refreshable Braille display. This is a row of Braille dots that raise or
[36:02] lower based on what the screen reader is reading out. Yes, some people aren't even hearing this aloud,
[36:12] they're just feeling it. >> Interesting. How would they be able to feel it then?
[36:23] Is that something that's like a different device? >> Yes. I said peripheral,
[36:29] so it's a device, like it's a piece of hardware you'd plug into your computer.
[36:34] Yes, the dots would raise or lower. >> That's really cool.
[36:40] >> I want to say like a quarter of day-in, day-out screen reader users use refreshable Braille displays.
[36:47] It's not an insignificant amount by any stretch. >> There we go.
[36:59] Braille? Actually. >> There we go.
[37:09] >> Whoa. >> It's definitely not very friendly on Google.
[37:32] >> Okay. >> I say that as it won't let you scroll and highlight something else.
[37:38] It was just pulling it back up here. I was wanting to scroll and then click on something.
[37:46] It wouldn't even go down here, it just kept pulling it back up to here and it wasn't.
[37:52] I have the same type of thing happened to me before on voice-to-text too. >> Yeah, absolutely.
[38:03] The tabbing that you saw, moving the focus. Again, focus is where your cursor basically is,
[38:12] like your keyboard cursor. It's the same for a screen reader.
[38:17] Now, remember that focus is only for interactive things. Actually, even specifically,
[38:24] focus is really only for things that you can interact with your keyboard. The idea is it's whatever element would start receiving keyboard events.
[38:32] But anything you can do with your mouse, you should be able to do with your keyboard.
[38:37] Therefore, we can broadly speaking say that focus goes to interactive things. If you think about it, you're going to miss content on this page,
[38:50] if the only thing you can do is go between interactive elements. You could go to the links,
[38:56] but you can't read the rest of the paragraph. You can't read the heading, for instance.
[38:59] >> Right. >> We need ways to access anything on our page.
[39:05] Static content, interactive content, stuff like that. The next screen reader navigation mode I'm going to
[39:12] introduce to you is called the virtual cursor. Here's how you're going to do this.
[39:18] When you turn your screen reader back on, you'll just click into the page once.
[39:24] I find I sometimes have to highlight the text a bit, or highlight a piece of text to get started.
[39:31] But then you'll do Control, Option, and then the left and right arrow keys.
[39:38] >> Which ones again? >> Control, Option, and then the left and right arrow keys.
[39:57] You're holding down Control and Option, and then you're going to use both of them,
[40:02] Control and Option, and then you'll use the left and right keys. Is it dinging at you?
[40:13] >> Yeah, I do. >> Okay. It's because your virtual cursor got trapped in a radio group.
[40:22] To get around this, I usually start by highlighting a little piece of text or something like that.
[40:27] >> Sorry, say that one more time. To get out of that, you get.
[40:32] >> I usually just highlight a piece of text with my mouse or something like that. That usually gets me. Okay.
[40:38] Now, let's try Control, Option, and arrow keys. >> Okay.
[41:00] That was fun. >> Yeah. But you can imagine that if you were reading something bigger,
[41:06] like a whole blog or a news article or something like that, that'd be inconvenient to have to keep progressing.
[41:12] >> I actually want to try this now. >> Okay. I encourage that.
[41:19] >> Yeah. >> Okay. Let's see.
[41:30] >> I know you guys can't hear this. I'm getting there.
[41:55] I'm getting there. >> We're good.
[41:58] >> It reading the title of this post that I made is star, star. What is a dev rel?
[42:18] What is an avocado? Avocado, avocado, avocado.
[42:22] >> Yeah. >> I love it.
[42:25] >> Yeah. Well, but this speaks to a bit of the user experience of using a screen reader.
[42:32] Because I don't want to say don't use emojis. But if a screen reader announces emojis,
[42:41] it can really clutter up the experience. This is where folks will advise,
[42:46] find a way to cut down on emoji usage. Don't have a whole wall of emojis
[42:52] because that can be an absolute pain to get through. In this case, it's star, star.
[42:58] What is a dev rel? What's with the avocados? Avocado, avocado, avocado.
[43:03] Maybe as far as screen reader users are concerned, like you could have been fine with just simply avocado at the end.
[43:11] >> Yeah. It's interesting that it did the stars because that was, and this is probably my need to look at the article anyway,
[43:20] it should be bolded or yeah, I think it's bolded or a title or something and it could have been
[43:26] just when I imported it, I didn't realize it. It definitely is something that I see only doing a few.
[43:40] >> Yeah. >> Because even doing this,
[43:43] if it says avocado, but I think it's also like I like that thing though.
[43:52] I like the claps. What happens if I, I'm switching screens now.
[43:57] >> Okay. >> I select over here.
[43:59] >> What do you think is going to happen? >> Yeah, I don't know how streamy art is on accessibility.
[44:16] Okay. Oh, hello. Yeah, I don't actually know where your cursor is.
[44:23] Do you want me to spoil it for you? >> It doesn't actually, just a sec.
[44:29] Oh, thank you. It makes it hard to talk and think at the same time. It doesn't, and what I was trying to see if it would do is read that comment.
[44:42] >> Yeah. >> It would not read the comment, even highlighting it.
[44:46] I ended up making my screen go full screen because I was trying to see if I can make it by showing it if it did it.
[44:57] That's very interesting to think about how not all applications are accessible.
[45:03] >> Yeah. No, absolutely. Do you want to put Anthony's comment on the screen again,
[45:09] so we can talk through this? >> Yes.
[45:11] >> I am pretty sure that the way that this announces is and clapping hands, don't clapping hands, don't clapping hands, this.
[45:18] Sorry, I think I missed the do. Do clapping hands, this clapping hands thing.
[45:22] Now, things get even worse if you've specified a skin tone modifier for the emojis.
[45:31] Because that's going to be, I think that would be and clapping hands with white skin tone modifier,
[45:38] don't clapping hands with white skin tone modifier, something like that, hugely, hugely cluttered.
[45:43] >> Interesting. Wow. >> Right. You can see how instantly what is cute for
[45:52] those of us who are sighted and don't have to use a screen reader to access the content, that's cute.
[45:58] But it's introduced so much clutter to the point, to the fact where it becomes very hard to actually decipher what's being said.
[46:10] Perhaps a more accessible version of that meme could have involved just putting one clapping emoji either at the beginning,
[46:20] or at the end, maybe at both, right? >> Yeah.
[46:24] >> Yeah. >> Interesting. This is making me think a lot about,
[46:31] and you and I talked about this a bit on our very first stream of a screen reader versus text-to-speech.
[46:40] >> Yeah. >> Even text-to-speech speeches have a hard time with emojis,
[46:49] and yet it's like how, oh, this is so complicated, I'm torn.
[46:56] That and I really do love emojis. >> I like them too, right?
[47:02] But I think the answer is it's not don't use emojis, it's use emojis in moderation.
[47:10] >> Yeah. >> Which is maybe disheartening to hear,
[47:15] but at very least it means that we're not introducing gobs of clutter to a screen reader user's experience.
[47:22] >> Yes. >> I want to express that I use emojis,
[47:27] I tweet out emojis, like I include them in my semantics announcements.
[47:30] This is absolutely not me putting the ban hammer down, putting the kibosh down.
[47:35] >> No, because you used a good emoji that I want to start using for the location.
[47:39] I was going to tell you that. I was like, that's a best practice, I got to use that.
[47:44] But I can see how it's just making me think. It's just crazy how when you don't realize these things,
[47:54] just to be very cognizant about them. >> A lot of folks aren't aware of this.
[48:01] A lot of the trending memes on Twitter are very emoji centric. A while back, there was a meme,
[48:09] you probably saw this one, the red flags meme on Twitter.
[48:13] The idea would be you describe a behavior that you find problematic in some way.
[48:23] Then afterwards, you would fill the rest of the tweet, whatever remains in your character limit,
[48:28] with red flag emojis. >> Ew.
[48:31] >> When they use TypeScript instead of JavaScript, red flag, red flag, red flag,
[48:40] red flag, for instance. But the issue is that screen readers, first of all,
[48:46] that's a ton of emojis, tons of clutter, and these tweets were everywhere.
[48:50] But second of all, there's nothing in the computer that says that that's specifically supposed to be a red flag emoji.
[48:58] In fact, the official name was like triangular flag on post. It wasn't even clear that it was supposed to be a red flag.
[49:05] It would be like when they use TypeScript instead of JavaScript, triangular flag on post,
[49:10] triangular flag on post, triangular flag on post,
[49:13] triangular flag on post. A lot of Twitter memes are emoji centric in a way that
[49:21] increase clutter and don't even really help in comprehension of what is actually supposed to be referred to.
[49:27] Mike, hello. >> Hello. Ben.
[49:34] >> Yes. >> Now, one day a video or a speech or a blog,
[49:41] something, a one-day idea for you, Ben, of screen reader versus text-to-speech.
[49:49] >> I got you. >> Because I would watch that,
[49:51] and I think that's something that I would share a lot about. I say it, I think this is a big,
[49:57] and I would love a call out on this. I think it's something that when these ideas pop up for me,
[50:02] I'm like, "Oh, let me share it with a person that does this. This is their jam."
[50:08] Because I'm like, I can write it. It's something I'd be very curious about,
[50:13] but it's not going to have the same impact than somebody that's in that space.
[50:17] >> Sure. >> I'm curious how that works.
[50:20] >> Yeah. Well, maybe we can continue our exploration of screen readers then.
[50:24] One of the things that it's been doing is, as you navigate to different things on the page,
[50:28] it'll tell you what kind of thing that is. That itself is a key difference
[50:32] between screen readers and text-to-speech, where text-to-speech will just say, "Submit,"
[50:37] but a screen reader will tell you it's a "Submit" button, for instance, or this right here is a link.
[50:44] Yeah. We had just finished talking about the virtual cursor, but I wanted to give you a shortcut so that you
[50:51] wouldn't have to keep Control-Option-Arrowing throughout the page. This is what we're going to call continuous reading mode.
[50:58] Continuous reading mode is Control-Option-A. Let's go ahead and turn voiceover back on,
[51:06] and then put your cursor somewhere and do Control-Option-A. >> I have to turn it back on.
[51:11] >> Yep. >> You said Control-Option-A?
[51:21] >> That's correct. >> I like this.
[51:48] >> Yeah? Tell me more. >> To do it as a comparison,
[52:02] I use an app that's text-to-speech called Natural Reader, I believe. I do like it,
[52:12] but it doesn't always know where to select, and it will a lot of times read this,
[52:20] and then skip down here. It makes it really difficult because, for example,
[52:27] I build all of mine in Notion, and when I was going through here and doing it with text-to-speech,
[52:41] it won't read the first line. I put a random first line here,
[52:47] so that way when I'm listening it back to myself, to make sure that I'm not missing something because I am really dyslexic,
[52:54] that it's reading the first paragraph. >> Screen readers are typically used by people who are blind or low vision,
[53:05] but I have also heard of screen readers, not even text-to-speech screen readers,
[53:09] being used by dyslexic people as well for very similar reasons, so just being able to read content aloud
[53:15] and get all the information about links and stuff like that. This may be something worth considering for you,
[53:20] if you find that this is working better than your current text-to-speech tools. >> Yeah, because I do really like the text-to-speech,
[53:26] and our comment about emojis has really made me think about emojis, and the fact that I do use them as my bullet points a lot,
[53:36] but at the same time, hearing how they're describing the screen reader or the emoji itself,
[53:43] it's like, "Okay, cool. How is that going to make a big impact if it's
[53:51] not the exact same visual representation as it is?" >> Sure, yeah.
[53:57] >> Some of them, this emoji is considered tears of joy, whereas that's what it's called,
[54:04] and I was like, I've never seen anyone use that as tears of joy. So it's been like a laughy emoji.
[54:11] >> Right. >> So in my mind,
[54:15] and I'd be curious for people that experience this, if context, how much context goes into it,
[54:23] and how often someone may work on consuming this content, or if they skip through content,
[54:32] what is that user experience like? >> Yeah, and a lot of emojis are very contextual.
[54:38] There's one example. There's one emoji that depicts a face that's like blowing steam out of their nose,
[54:47] and so many people in the West will use that as an anger emoji. But this is actually,
[54:58] if you look at the name of the emoji, it's determined face because the notion of having steam coming out your nose.
[55:08] In Japan, from what I understand, and Japan is where the first set of emojis came from,
[55:13] that's the standard cartoony depiction of determination. So people are using a thing like an emoji that looks a certain way,
[55:23] in a way that doesn't quite connect to the underlying name of the emoji, and there's cultural connotations there too.
[55:31] So a screen reader user is going to hear like determined face, which isn't quite the same as face that's steaming with anger.
[55:42] That's the one. Yes. >> Yes. Interesting.
[55:49] This is so fascinating and I know we're getting close on time, and I just want to say that Ben,
[55:58] I feel like you need to be a monthly visitor because you just teach us so much about as we're developing things and it's not just a developer aspect of it.
[56:10] I feel like accessibility is something we need to think about throughout everything that we're building,
[56:15] even as it comes down to APIs. >> Yeah.
[56:19] >> So now I'm like mind boggled again. >> I'm down to be a monthly guest.
[56:25] But with this little bit of time we've got, can I show you one more thing with screen readers?
[56:29] >> Yes. >> Then I think in months to come,
[56:35] we'll start talking a lot more about semantic HTML, semantic markup because I think that's a huge part
[56:40] of a strong foundation for accessibility. But let's go back to the Dev 2 page,
[56:46] and we can use that as our grounds here. What I'm about to introduce you to.
[56:53] In VoiceOver, it's a feature called the rotor. Different screen readers all have
[56:58] their own implementations for something like this. I think that VoiceOver is the easiest to use,
[57:03] especially for us sighted testers. But the idea is,
[57:07] it's going to be a way to navigate between different elements of a similar type. So that could be like going from heading to
[57:17] heading or link to link, button to button. In JAWS, NVDA, Narrator,
[57:23] those are other screen readers, they all have keyboard shortcuts for this.
[57:26] But I find that VoiceOver is going to be the easiest because it packs everything into one nice, easy shortcut.
[57:33] The way we're going to do this is we're going to turn VoiceOver back on, and then you're going to do Control Option U.
[57:41] >> Go ahead and do the up and down arrow keys a few times. >> Hi.
[58:03] >> Yeah. Hello. >> Sorry?
[58:06] >> Yeah. Go ahead and hit up and down a few times. >> Okay.
[58:12] >> So yeah, you're skipping through the page going from link to link. >> Sorry, one more time?
[58:20] >> You're skipping from the page going from link to link, right? >> Yes.
[58:24] >> So you can imagine, if someone's included a bunch of links that are all called click here or read more,
[58:31] well, this is a very valid way to navigate the page that is completely taking those links out of context.
[58:37] >> It is. >> So this is one of the reason that accessibility advocates
[58:45] will recommend that you keep your links very specific and to the point and descriptive. Your link should describe where they go,
[58:54] because in a mode like this, you don't know where they're going to go.
[58:57] You don't even know the surrounding context. >> So on that note,
[59:03] if I scroll all the way down, if I were to put this link in what's with the avocado and linked it there,
[59:14] they would at least know that that link has something to do with what's with the avocado.
[59:19] >> Yes. >> Instead of click here,
[59:21] then click here just would mean we have no idea, but it is actually embedded with the text of it.
[59:29] >> Yeah. Let's real quick hop back into the voiceover and hit the left and right arrow keys to go to different panels.
[59:37] The panel that I want to especially highlight is the headings panel. >> It's control option U.
[59:46] >> Yeah. Nice. Here we go. Can you hear me by the way? Can you hear me?
[59:59] >> Yeah. >> Awesome. What this is doing is this is giving us
[60:03] all of our H1s through H6s on the page. >> Oh, that's cool.
[60:09] >> Yeah. It even tells you which heading level. The one that your cursor is on right now is an H1.
[60:15] If you were to go down one, it would take you to do an H2.
[60:18] >> I would say the only thing that especially if people are having a hard time with visualization,
[60:31] but can still see is it would be cool if it scrolled to where it is on the page. >> Sure.
[60:38] >> This is so dope. >> Yeah. You can hit "Enter" by the way,
[60:44] if you want to close the rotor and scroll down to it. There you go. Now we're starting to see how the elements that we use
[60:52] impact how this experience is presented to assistive technology. Folks who are not sighted,
[61:02] you and I, we're sighted. If we're looking at a page and we want to get a piece of information on that page,
[61:09] we might skim through the page until we find a heading that seems roughly right and then start reading more closely.
[61:14] But a screen reader, when you just use the virtual cursor, is inherently linear.
[61:21] This is effectively giving screen reader users that same skimming functionality. Unfortunately.
[61:30] >> I know. You have to jump. Thank you. We look forward to having you on again soon. Bye, everyone.
[61:37] >> Bye, y'all. 
