---
showLink: "https://www.youtube.com/watch?v=hcqZCaOZwCA"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-open-source-contribution-with-guests-taylor-fairbank-ram-n-huidobro"
title: "Teach Jenn Open-Source Contribution with guests Taylor Fairbank & Ramón Huidobro"
publishDate: "2022-08-30"
coverImage: "https://i.ytimg.com/vi/hcqZCaOZwCA/maxresdefault.jpg"
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

[00:00] >> Hello, hello, beautiful humans. Welcome back to the collab with Borderless Dev.
[00:09] Taylor is the real name, not just Borderless Dev of the Twitter names.
[00:16] I am half asleep this morning, if anybody was wondering,
[00:21] which Taylor is currently across the world, so wide awake.
[00:27] Who I was just talking to, they were in France and wide awake.
[00:30] It's the afternoon, evening there and I'm like, I'm struggling just waking up.
[00:35] >> We have the advantage of being later in the day. We got the right time zone shift.
[00:41] >> Yes. Well, thank you again for joining Teach Gen Tech and Distribute Aid in letting us tinker
[00:47] around and learn so much while doing this together. Because not everybody has seen previous streams with you and Ramon,
[00:56] can you give us the download of what Distribute Aid is? >> Totally. Hey, everyone.
[01:04] It's great to meet you. I'm Taylor, he/him, Borderless Dev on Twitter.
[01:09] Distribute Aid is the world's largest grassroots humanitarian aid supply chain. We work with over 140 small informal organizations, charities,
[01:22] community groups to help them collect aid, ship that aid to frontline organizations,
[01:31] get it parceled out to where it's needed to go, and then those frontline organizations will distribute it.
[01:37] We also work with large global freight forwarders and large companies who want to make in-kind donations.
[01:45] But our heart and soul is that grassroots community. The idea is, can we make the complex global supply chain stuff easy for
[01:54] community groups and connects communities around the world through this physical supply chain,
[01:59] with the focus on just everyday people helping everyday people. Cool. Thanks so much for showing off our stuff.
[02:07] That's our landing site which we're going to be hacking on. You can see some of our work right there.
[02:12] But one of the big problems we have is we do so much work. We shipped $14.7 million worth of aid over the past 12 months.
[02:23] We want to make that visible. We want to make that accessible.
[02:26] We're doing all this great work. We want to show it off on our landing site,
[02:29] make it easier for people to tap in to the Distribute Aid Network, and show all this great community-driven work to show people that it's possible,
[02:42] and that they too can collect aid or distribute aid in their communities, or ship it abroad to respond to a crisis in the country they care about overseas.
[02:52] We don't need anyone's permission to help out. >> You break it down to being a very consumable way,
[03:04] not only what Distribute Aid does, but also since we've been collabing together and also with
[03:13] Ramon of learning the process of contributing to open source. Now, quick question because I know we talked about this a little bit last week.
[03:29] How would you, and hello, Noelle, I do see you.
[03:33] I'm just deep into the thought process. How would you explain what supply chain is and a bit about if people,
[03:48] so this is my concept of it, is you grab some stuff and you give it to
[03:54] a community or a company and they distribute it everywhere. Now, I guess I don't see how this will break down.
[04:08] What up, Hexil? I'm going to work on saying your name.
[04:14] What up, Ben? >> What up, everybody? Thanks for reading off the comments.
[04:19] I only have one monitor, so I can't see the- >> I got you.
[04:23] >> -stream or anything. Yeah, it's good to see you all in the channel.
[04:27] By the way, as we're going through and doing the coding and stuff, y'all, I don't know everything,
[04:31] Jen don't know everything, we're here learning together. Please feel free, help us get unstuck,
[04:37] help us look up documentation. Let's make this a little bit more interactive,
[04:42] not just a passive viewing experience. Contributions are welcome.
[04:45] >> Yes. That being said, please share with your friends to tell them to come watch the stream.
[04:52] I'm like, I don't know if I'm allowed to say that. Even if it's on mute in the background,
[04:56] because I got to get to three average streams. Three people per average streams.
[05:04] I'm like, "Why? Why? Why? Why?" I don't know.
[05:08] >> I don't know. It's not like some Twitch work thing. >> Well, it's like you can't become an affiliate
[05:13] without an affiliate is where you can do donations. I've had people reach out and be like,
[05:19] "Why can't I subscribe to your channel? I want to help your channel."
[05:23] I'm like, me asking Ben a lot of questions yesterday of why not. Please share, even if they're watching in the background, that is cool.
[05:34] Back to what is Supply Chain? >> What is Supply Chain? Let me break it
[05:42] down with a real example from one of our regular routes. We're the team that solved Brexit for sending
[05:50] aid between the United Kingdom and northern France, which was disrupted.
[05:56] We had to work closely with French customs. It's supposed to be legal to import
[06:01] aid tax-free to these European countries. If the process is actually in place or not is a different matter.
[06:08] Government says one thing, does something else, and so we had to help them bridge that gap.
[06:13] We've been running a truck every six weeks or so on this regular route. What it looks like is started a timeline,
[06:22] we got six weeks before we want it delivered. We take the needs data we've collected.
[06:28] That's actually powered by some of our open-source tech. We have these needs assessment surveys that
[06:33] project needs for a few months in the future. It's like, "Hey, we're talking to groups,
[06:37] we hear about some needs, we're taking the data they give us and pushing all that together."
[06:42] We go advertise those needs to our community partners in the UK, potentially some in-kind donors that are on our radar, things like that.
[06:51] They then make offers. That's done through our landing site on the regular routes page.
[06:57] I'd love to upgrade this at some point. Right now, it's just an Excel file.
[07:00] You download the Excel file, you fill it out, you submit it.
[07:04] Wouldn't that be great to automate, have native through the website or some other online tool?
[07:12] But yeah, we take the offers and we do a double confirmation step. We then present them to the frontline organizations.
[07:20] On average, you might have 10 groups making an offer. I think we have six or so partners in Northern France.
[07:27] They get to choose the aid. This really makes sure that we never ship aid that's not needed.
[07:33] We don't want to send trash, we don't want to send items that aren't useful,
[07:36] that'll sit in a warehouse. It's like, "Hey, what do you need for the next six weeks until
[07:40] the next truck and then we'll do this all again?" Sensors, we're just sending what's needed.
[07:46] It's very high quality and that takes about two weeks right there. Then we have four weeks now to go back to the sending groups and like,
[07:56] "Right, here is the aid that was selected. Please get that to the staging hub."
[08:01] We also start planning the shipment. All these community organizations are
[08:05] doing a fan run or throwing stuff in there. It's the case, they don't have pickups,
[08:10] but Americans in the audience, imagine throwing a bunch of boxes in the back of your pickup,
[08:14] like doing a few runs to the staging hub. The warehousing folks we work with are another charity group.
[08:21] Sometimes we bring in volunteer teams from some of our partners to package those boxes up into pallets.
[08:28] I don't know. I think people are familiar with pallets. It's those wooden things.
[08:33] You put a bunch of boxes on them and then you surround wrap them together. We have some optimizations so
[08:42] that we're palletizing stuff for a single receiving group. We can plan that out because we know where that aid is going.
[08:51] In the meantime, our logistics coordinators are working with very big global freight forwarders to book the actual trucking.
[08:59] It's got to pick up here on this day, here's the weight and the volume of the goods we're moving.
[09:04] We're also working with export customs in the UK, import side customs in France,
[09:11] and applying for tax exemption status. Because this is all coming from people for free,
[09:17] going to people for free, it's humanitarian aid.
[09:22] We don't want to have to charge our community partners more, give the government a cut when that same government
[09:30] is violently evicting the people we're trying to serve. It just doesn't make sense.
[09:37] There are lots of moving parts there. But the basic idea is we work with all these community groups on
[09:43] either end as this bundling idea. That way we help these community groups scale up their efforts by
[09:51] working together in order to tap into the shipping at scale to get efficient pricing.
[10:00] I think on that route, it's probably about, if I had to guess right now,
[10:06] I'd say 200 pounds, maybe $250 to move a pallet of
[10:10] aid if you take it personally in your car or in your van or something. I'm not saying people shouldn't do that.
[10:16] It's important to have connections and visit the folks you're supporting once in a while.
[10:20] You don't need to do that every month. For us, we charge right now 75 pounds.
[10:26] It's about $100 per pallet. We're cutting those costs in half.
[10:32] We're also doing this regularly. That means that the frontline groups know, "Hey,
[10:38] the next distribute aid truck is coming in six weeks." It takes a lot of pressure off of them.
[10:43] When that truck arrives, we drop off some pallets at one of the hubs, which is then those pallets are split up and get to the local groups there.
[10:51] Then we have a second hub. The truck goes a little bit further,
[10:53] drops it off for the groups over there. Does that make sense in terms of-
[10:57] >> It does. >> -all the different pieces?
[11:00] >> Yes. I don't know if you can do this post, but I'm going to go do a best practice that Ben was doing,
[11:10] make a clip out of that. Because I think the way you explained that was super dope,
[11:14] and it's something that you can reuse, but we'll see if Twitch does that.
[11:18] I don't know yet. What up, Anthony and Bakari? Yay, so many more people.
[11:25] Can I share it out to get more followers on here or streamers? Because I need people watching it.
[11:32] Now, we got the background on it, which has been some curiosity questions that I've had.
[11:40] Thank you, Anthony. I didn't mean in Twitch though. That is good. StreamYard makes YouTube happy.
[11:51] I'm saying it because I'm almost to that affiliate level. All I need is three average viewers per episode,
[12:00] and I'm at 2.5, and I think I hit 50 followers.
[12:04] I'm not sure yet, but that's a story for another time. I do appreciate everybody sharing that out.
[12:11] I will see if I can remember how we got around on getting everything set up,
[12:21] and see if I can explain this well as I go. All right. I'm a little nervous,
[12:28] little excited, so we'll see. As Taylor explained what Distribute Aid is,
[12:36] there are a lot of different people within the organization that need to have
[12:42] access and make changes to the website, yet the marketing site,
[12:47] yet it can be a bit too complex for people that don't know how to
[12:50] code or don't understand it very well. The goal of what we're working on is to make a template page.
[13:01] I mentioned that before I go over to GitHub, because I'm like, okay, cool.
[13:06] From a non-coding point of view, I can comprehend that pretty easily.
[13:11] I'm going to open a fancy new tab and go to GitHub. Throughout the last two times that we streamed,
[13:23] because this has become a long-term collab. We have, I'm going to scroll down.
[13:31] We do have a really good read-me here, which really describes what we're using.
[13:37] Gitpod is what we use to be able to edit everything. But if you scroll down,
[13:44] I do really want to find this and point it out. Where did the map go?
[13:53] Is it not in here anymore? >> The code-based map? It should be there.
[13:57] I think the link you found was about CodeCMaps. But if you scroll to the top, there's the-
[14:03] >> Oh, it's just on this. It made it look like it was just some random title.
[14:09] >> That's interesting. I might need to make that more accessible by highlighting that it's a clickable thing.
[14:15] >> Yeah. This one makes it go, okay, that's definitely a button.
[14:19] Where this one, I don't know. >> It's like a little banner or something.
[14:23] >> Yeah. I don't even know if you can make that and mark down, but to be that way,
[14:26] so I would think I'd know that. So CodeC, okay.
[14:32] I need to remember to start doing this command-clicking stuff so it doesn't-
[14:36] >> Yeah, it's a GitHub thing where they- >> Drives me bonkers.
[14:40] >> Yeah. >> Yeah, I was looking into this one
[14:45] because it should be able to show you the CodeC map without needing a CodeC login.
[14:54] So I was trying to make it more accessible that way. We set that up a while ago before we had
[15:00] the DistributeAid team account on CodeC. So yeah, I might need to make that a bit easier there.
[15:09] >> Well, we don't necessarily need CodeC, we'll find it another day.
[15:14] >> Yeah, there's other CodeC stuff like in the issue, for example. There's a CodeC map in the issue, yeah.
[15:20] >> Cool, then we'll go take a look at that one. Hoxiel said, "Yeah, it does look like a badge."
[15:30] Anthony said, "By the way, Taylor, I don't know if you're looking for a payment solution,
[15:37] but my friend runs a startup focused around taking donations for nonprofits."
[15:41] >> That's awesome. We are looking for donations. You can go to distributeaid.org/donate.
[15:46] We currently use Open Collective for US donations and Patreon or
[15:52] bank transfer for international donations. >> Website, donate.
[15:58] >> Yeah, you got all the different channels right there. Yeah, I'm always interested in talking to startup people,
[16:06] so please send me a DM on Twitter. I'm at borderless_dev and point out their startup.
[16:12] I'll definitely check them out. But it's something that we also have other channels for.
[16:19] I don't want to make any promises here on stream. I'm in the hot seat, right? I'm live right now.
[16:23] >> I get it. You're like, maybe, you never know. But I do think it's cool.
[16:29] They said, Anthony, you're like they. Anthony said, "Okay,
[16:35] they might be able to help with bank transfers." Which I think is pretty cool because the world of
[16:40] FinTech is just so expansive. I found another Jannad on LinkedIn.
[16:50] I was just like, "You're a Jannad? I've never seen a Jannad in the wild."
[16:54] I added him on LinkedIn and he's like a CTO for a bank, like a startup bank.
[17:00] I'm like, "This is cool. FinTech is just so fun."
[17:05] I also have a really fun time of asking people from Stripe, why are they so square?
[17:15] >> That's really funny because I have a friend who worked at Stripe who was an amazing friend but also kind of square.
[17:22] >> Yeah. Luckily, the guy was cool with it. We went through the code me,
[17:27] we're going to the issues. I have this issue that I slightly blame
[17:34] Taylor because he made a giant issue. >> That's how you get someone hooked and then
[17:41] give them more to keep contributing to, right? >> Let's see if this code C works.
[17:48] >> Yeah, this might be the shorter way to try to explain what we're doing here.
[17:54] >> Yay. >> We have the tour and everything.
[17:57] >> Bakari said, "Dad jokes coming through strong." If anybody wants to share dad jokes or puns with me,
[18:05] please tag me because I find them freaking hilarious. Ben said, "My past role was web dev for a bank and man,
[18:14] I wanted out of anything to do with banking financing regulations." Dude, our last API Denver Meetup was sponsored by JP Morgan.
[18:27] They were like, there's so many regulations. >> Yeah. It's like supply chains,
[18:34] but there's a lot of things that you're supposed to do in supply chains,
[18:37] but it's more like suggestions or best practices. It's amazing that anything actually
[18:41] ends up on the grocery store shelves. >> That is crazy.
[18:46] Anthony said that he's reading a book about the life of Henry Ford.
[18:53] I was like, that's very interesting. >> No, that's a dad joke right there.
[18:57] It's an autobiography. >> Autobiography. Yeah, I love it.
[19:02] >> Sometimes they do go over my head. I will say that.
[19:06] Although yesterday, Anthony said on his live stream that he's got to stay hip and that one was just making me
[19:13] laugh really hard when he shared the video. Anyway, to focus back on,
[19:19] let me make this bigger too. Let's see if I also remember this.
[19:27] CodeC is where they show you what it looks like in a mind map view instead of the file format.
[19:39] >> Yeah. It shows the dependencies between things rather than just, here's this folder and you don't know how
[19:45] files relate to each other and stuff. >> These are all files outside of the source folder and then you have pages.
[19:57] If I follow this right, source, then pages, then layouts.
[20:02] Layouts is within pages. >> All those files are within source.
[20:08] >> Source, okay. >> It's source/pages, source/layouts.
[20:11] But if you click on "Pages" right there, it'll show you that there are files in pages,
[20:21] like there are different pages that call out to layouts, which makes a lot of sense.
[20:27] We set up when we were coding this generic page, we use the simple layout.
[20:33] It's telling you, hey, some of the files in the pages folder are
[20:37] using layouts or components or other things. >> I think this is a really great way for newbies to get started,
[20:46] and why I really like the idea of working with distributed and learning open-source,
[20:53] because this is a way to build that mental map of how things are going. Another open-source that we'll be having on the show to talk
[21:03] about is going to be open-sauced with BDougie. Thank you, Anthony. He did reply.
[21:10] We have him booked on the show, so he'll be coming on later this month.
[21:15] I like seeing how different open-sources are very similar yet so different.
[21:23] Going back to our wonderful, wonderful, very giant thing to do.
[21:37] Sorry. Sorry, I just put a funny joke. You know why I don't like coding well on a boat?
[21:45] Too many dependencies. I like it. This just seems to be what we do on all the live streams is funny jokes.
[21:55] This is the absolute giant thing to do. I'm scrolling down to the bottom just because I am trying to do
[22:04] a quicker recap of when these issues are made, mattering on the open-source,
[22:10] you may want to see if you can be assigned it. It really does matter.
[22:16] Look at the README, reach out to the organizer? >> Yeah, the maintainer.
[22:23] >> The maintainer, thank you. >> Look through the issues,
[22:25] and if you feel like you want to tackle something, just leave a comment. Just like, "Hey,
[22:29] hello, I think I want to try my hand at this." They can assign you to the issue to communicate
[22:35] to folks like you're actively working on it. Yeah, I think have that conversation around the issue for sure.
[22:43] >> I do want to point out something that I think is a really cool best practice that's on open-source and on this one,
[22:51] is you can see if it's a bug or help wanted or when they're tagged. This is a really cool way of doing it as well as you can
[23:02] see who is assigned to it, any comments. Y'all, I don't know what that was for a while.
[23:09] This is where I'm going to get a little iffy. Pull request, create page template, which is mine.
[23:19] >> Yeah. >> Hey, CodeSummit.
[23:23] >> These are the changes. >> Oh, that's fine.
[23:26] >> This is one of the diff maps. You have your work in progress or draft pull request,
[23:31] which is great, highly recommend that. Y'all, make your first commit on a branch,
[23:36] push it up and on GitHub, you can make a draft pull request.
[23:40] On GitLab, you can make a work in progress pull request. This gets your code that you're working on.
[23:46] You don't have to do everything by yourself. Get it out there early so you can ask for feedback,
[23:51] you can ask questions. This gives you a space to share your work while you're still adding to
[23:57] that pull request and communicate with other people involved in the project.
[24:03] I remember when I was still learning how to code, I'd want to have everything perfect and have
[24:09] my perfect little series of commits that solves the issue before sharing it. But that just meant I spent a lot of time by myself,
[24:17] which limited the amount that I could learn or that I had run into issues that I couldn't answer and then gave up.
[24:25] Don't be afraid to push it up there early and just mark it as a draft so that people know it's not ready to merge in yet.
[24:32] >> I feel like I need to ask more questions about that eventually at the moment. What you're saying makes sense,
[24:39] but it doesn't make sense. This is the weird thing about tech,
[24:43] is it's like it's so simple, yet why does it not make sense?
[24:47] Ben just shared that he's never seen used code C before and it is really cool.
[24:57] I clicked on another one without reading it. Seriously, time and again,
[25:05] I rediscovered how important it is to open the pull requests early and get early feedback.
[25:10] >> All right. I am slowly looking for how to get in to not code C, but the other one that we were using.
[25:27] >> Gitpod. >> Yeah.
[25:29] >> That's in the README there. >> Is the README the only place you can get to Gitpod from?
[25:37] >> I think so. >> That's usually when Ramon and I do it,
[25:41] we open the Gitpod and then dive into the issues and the pull requests and stuff.
[25:47] >> It could be cool. I don't know if this is a part of the setup if they do it, but it could be cool if they had something in here of when you
[25:55] create a PR that it puts the link in there, because now I'm like, "Okay,
[26:01] let me not lose where I was." >> Yeah, I feel you.
[26:06] >> But we now know that this is not a banner, it is a button. >> Right. That's worse up there.
[26:13] We got to fix the link so it's not logged in. >> Then I just click.
[26:18] >> You did it from the issue. Remember the README one requires you to be logged in to code C with Distribute Aid.
[26:28] It's not shared publicly, which is an issue in our end, so I'm trying to.
[26:32] >> Oh, yeah. Okay. That's what I did. >> There we go.
[26:34] >> Okay. Yay, continue with GitHub. If anyone wants to know something really funny on my second stream or third stream,
[26:45] Anthony, I don't remember which one it was. I set up my GitHub account,
[26:50] but I didn't know the login and I didn't know we were going to need it. I'm live-streaming going, "I don't remember.
[27:00] I don't know. Oh my gosh." Anyway. Second, yes.
[27:06] One of the really cool parts about doing this live is, it's a lot easier for people to pick up where you were,
[27:18] but then also, what is that? It looks so weird. >> It looks like the styles didn't load.
[27:24] I might give it a refresh real quick. >> Okay. There we go.
[27:31] >> There we go. >> Yay. But also,
[27:36] when you started taking over at the end of our last stream, Taylor, it was really cool watching him do stuff
[27:45] actually fast compared to me working on something. From here, I know I need my terminal.
[27:59] I need to open my PR. That's the thing. I don't remember how to do that.
[28:13] >> That's okay. Let's go take a look at the PR real quick, because I don't want to just give you the answer.
[28:20] I want to show you how you can find it for yourself. You have a PR you're working on.
[28:26] There's something about the PR that we need to open on Git. There we go. That's the branch is what that's called.
[28:41] Git has the series. It was like the main branch,
[28:44] which in our case is called Saga. Then you can create different branches and make commits onto them.
[28:51] >> Would it be the same file folder structure of going from CD to change it, or is it something else to change branches?
[29:03] >> Almost. You're going to use a Git commands, because the branches aren't in the file system.
[29:09] They change the file system. They're like different versions of it.
[29:13] You want to do Git checkout space and then the branch name. If you just start typing 523 or whatever,
[29:22] you can also tab to auto-complete. >> I copied it. Let me go back.
[29:33] Gabby. Let's see. Anthony just said,
[29:59] I should reach out to Pauline from Gitpod. That would be cool.
[30:06] >> Yeah. >> That would be really cool.
[30:09] Yes. For everyone should go follow Pauline, and I will follow up and go follow Pauline as well.
[30:19] We have it in the terminal now, that now we can go into the files and go look at things?
[30:26] >> Exactly. Yeah. Now you're on your branch, where you are working on this stuff.
[30:33] >> Pages, and then we made. It wasn't pages, right? That we made the page template.
[30:43] >> Yeah. There we go. >> All right. Then we can move this, and we can move this.
[30:48] >> Just so the audience knows our approach here, we're working front to back.
[30:52] We're starting by hard-coding content on the page, doing some styling,
[30:58] and then we'll continuously refactor that out. Our goal is to end up with these sections,
[31:04] which determine the layout of different parts of the page and content blocks in those sections.
[31:10] That way, in our content management system, you can imagine our admin or ops folks saying like, "Cool.
[31:17] I have a page, I want centered section with a text content block,
[31:23] and then I want a side-by-side two-column section with more text and an image,
[31:28] and then I want a grid with a couple of different visualizations or photos or something."
[31:34] If we give them the building blocks like the Legos, they can put the page together dynamically
[31:40] without having to ask us to do all that stitching. >> I'm just excited that this is day two of people mentioning Legos.
[31:48] One of these live streams, I'm just going to be playing with Legos.
[31:52] All right. I remember what we did was we copy and pasted one of the pages.
[31:59] For my own visualization, I was like, "What page do I want to choose?"
[32:05] When we were going through this and choosing which page to copy the code from,
[32:11] we decided on code of conduct and work from there. It was really helpful for me since I'm
[32:19] not a 100 percent in the coding area yet mind-wise, to see it visually then to be able to go to this.
[32:28] I just realized this is over here, I should move it to another screen.
[32:31] Y'all don't need to see that. Not that I care, but all right.
[32:38] >> On that note, why don't we go ahead and open up this page, so we can see our work so far on the browser.
[32:48] >> That was this, I think. No. I can't see because
[32:56] I need to really pay attention to this corner. I thought it was clicking the button.
[33:01] >> I thought it was. Yeah, I remember you clicked that maybe. >> Oh, it's the globe.
[33:04] >> There we go. Very cool. Now you'll need to navigate to the page.
[33:10] We're not linking to it anywhere yet, so you'll just want to do that directly.
[33:15] >> Oh, weird. I thought it did it last time. >> No, you're right.
[33:22] You just need to add slash page dash template there. >> Yeah, I just thought it did it last time by itself.
[33:30] >> There we go. That's where we left it off. We had two different content sections.
[33:40] The first one is that centered one. The next one is a two-column side-by-side.
[33:46] We have three different types of content blocks. There's a YouTube embed,
[33:51] there's a markdown paragraph, and there's an image.
[33:56] This is already making some decent progress here. >> I feel like something that could be cool is we
[34:05] have what I added on there just to see if we got text on screen of Hello Beautiful Human.
[34:10] Request to figure it out really quick would be just to censure that and make it a header.
[34:17] >> Totally. Let's have that be another type of content section, content block.
[34:28] >> Yeah. >> Let's take a look because right now it's just on H1 there.
[34:35] >> Wouldn't H1 show as a header and it's not showing as a header? It looks like small text.
[34:42] >> It does. The strategy Tailwind uses is to basically remove all of the default browser styles,
[34:50] because it wants you to explicitly choose those and style those here.
[34:55] >> If I did, let's see, just to copy your formatting.
[35:07] >> Maybe let's do single content, but let's try to have it left-aligned
[35:13] just to add some variety in there. Single content, left-aligned.
[35:18] That way the header will be on the left-hand side here, and then it can have centered or it can have side-by-side,
[35:25] things like that. >> I think this is something that I asked you last time,
[35:31] so please help with a refresher. For everybody watching right now,
[35:38] I think this is a great way. I'm curious how you-all do it too.
[35:41] How do you know what language you're looking at without, if you're not looking at an import or anything,
[35:48] is there just things that you see that you're like, this is Tailwind or this is TypeScripts or Python,
[35:55] or I don't know, I'm just throwing out a lot of random stuff now. >> Totally. For me, I think for something like Tailwind,
[36:02] that's a lot harder. What I'd usually look at is the readme or
[36:07] maybe the package.json to see what style we're including. The reason that's harder is because the only thing
[36:14] we'll see for Tailwind is this class names. But if I wasn't quite sure what the Tailwind class names were,
[36:21] it could be Bootstrap, it could be any other style library
[36:24] that uses a class name-based system. I like looking at the readme,
[36:28] hopefully developers left documentation there, or at the package.json to see if I
[36:33] recognize one of the style frameworks I'm used to. For languages like TypeScripts or React,
[36:40] I think those are a bit more obvious sometimes. This looks like React to me.
[36:47] We have the JSX or in this case, the TSX. It's making a component.
[36:52] There's some JavaScript intermingled with the HTML look and stuff. To me, I picked that up as React.
[37:00] Then for TypeScripts, it's because of that weird additional syntax.
[37:06] I pay attention to that. Like what is this colon FC thing on some of the other files?
[37:12] There's also like, hey, this is a string or this is something else,
[37:16] which shows me that there's type information involved in that. But I think the reliable way is like look at imports,
[37:22] look at the package.json file to see what the project's including, and look at the developer documentation.
[37:30] You shouldn't have to guess. >> That's something that I'm slowly getting better at.
[37:37] Here's some responses from our audience, viewers, team, friends.
[37:46] >> Our friends. >> Our beautiful humans listening.
[37:50] Y'all, I don't know what to call you. You're just awesome. Anthony said, Tailwind is in a language,
[37:57] it's a CSS library, so that's a little different.
[38:00] It's a dependency, not a language. He appreciated that you shouted out the readme.
[38:07] That is something Anthony has been working on getting me to create and to use, which I am learning, I am learning.
[38:16] TypeScript will also be in the package.json, so you'll have a TS and TSX file.
[38:26] Then I'm going to skip one just so that way I can keep them in order. React will also have JSX and TSX instead of JS and TS.
[38:38] Hopefully, Redwood's bad at this. Then Hockzeal said,
[38:46] "Syntax for Tailwind being so explicit is a good way to differentiate it." >> Thank you.
[39:00] >> That definitely works. If I see another project using Tailwind and Tailwind's syntax style, I'll pick up on that.
[39:08] But if you don't know what Tailwind is and you're just like, if you're more used to Bootstrap or something else,
[39:14] you might not be able to. That's where I think the reliable way is going back to that package.json file,
[39:20] that readme, and the imports and stuff sometimes. >> Sweet. For responses of what to call the viewers is homies,
[39:32] chat peeps, hood mob. >> Can I say beautiful humans of the hood mob, homies, peeps?
[39:46] We'll just keep explaining. >> The salesperson in me wants to call them future contributors.
[39:52] >> Well, everybody has been on the show so far except Hockzeal. They contributed to Teach Gen Tech.
[40:05] >> There we go. >> Wow. Viewer epitaph proposal cowards.
[40:13] Fucking cowards. All right. I know we don't have a ton of time here and I'm
[40:21] getting way too distracted from the chat because they're fun. We said that it's going to be single content left-aligned.
[40:29] Then because you said Tailwind removes all of the formatting, I would then basically just go Google Tailwind header.
[40:44] >> Yeah. That's a good way or just the Tailwind base styles. What is a header?
[40:49] You're bumping up the font size, you're making it bold,
[40:52] you might have an underline or something like that. So yeah, this is what they're saying,
[41:04] where basically it's removing the styles for Tailwind and stuff like that.
[41:11] So let's think about how do we want to make our title stand out? That's the Tailwind philosophy.
[41:16] It's like figure out what you want for your site's unique style and look and feel and stuff,
[41:22] and then use CSS to achieve that rather than taking something that is already opinionated and modifying it.
[41:32] >> I'm also staring at this and especially where it says margin and padding.
[41:41] I know this is skipping around a bit, but would we add margin and padding if we wanted to
[41:47] put between these? Would that be margin and padding?
[41:57] >> Yeah, definitely. That might be at the section level rather than the content level.
[42:02] We want to separate sections with each other and then the content. Sometimes we might need that, sometimes we might not.
[42:11] But definitely, probably margin for blank space between them. Padding would be important if we wanted to have the background color,
[42:21] like if we added a background color or something and wanted that to extend the text.
[42:24] One is for between things, one is for within the inner content and the border of the wrapper there.
[42:33] >> I'm not seeing it in here itself, which I know we have limited time,
[42:41] so I might just ask you on this one. How would I create this to be a left aligned?
[42:49] >> Totally. I think the first thing that we want to do here is we want to give it a quick wrapper.
[42:58] Let's look at that single content centered. There's the section class name,
[43:04] justify center. To me, that sounds like we can do something similar there.
[43:10] Instead of justify center, maybe we do justify left.
[43:14] That's our control to move it left or right using Flexbox here. >> It just gave me the other half.
[43:27] I was like, where did that come from? Thank you. For now.
[43:37] >> Perfect. Then the other bit we have there is this div. This div is controlling the size.
[43:44] We probably want to copy that just for consistency's sake and wrap the h1 in that.
[43:52] That way, it'll line up with the content boundaries that we've set for the video and other things.
[44:00] >> It didn't close my div. That was weird. >> Nice.
[44:10] >> I need to do some tabs because this is making it look really complicated.
[44:17] >> Perfect. That sets out our layout there. The layout is going to say,
[44:23] we want this in its own layer vertically. It's separate from the other content.
[44:28] We want it on the left-hand side. Maybe if you're on a larger screen,
[44:32] we don't want it to go all the way to the edges. We want to set a max width there.
[44:36] That's looking pretty good. Now, we need to actually style the header.
[44:40] Let's go ahead and add class name to the header, give ourselves some space,
[44:45] and then we can go look up some Tailwind classes as well. >> We would add another class name or?
[44:57] >> Yeah. In the h1 tag, you'd want to add the class name attribute.
[45:01] We're not exactly sure what classes we need just yet, but we know we're going to need to. You still want it to be h1.
[45:09] You want the h1 tag and then add a space there, and then this would be an attribute.
[45:16] Perfect. >> Like this?
[45:19] >> Exactly. >> Anthony said, Tailwind could be another topic on the show.
[45:27] I completely agree. At some point, anybody want to come talk about Tailwind,
[45:33] let's do this. We are going to look at h1 class names. >> Exactly. Let's think.
[45:44] Do you want your header to be a larger font size? Yes, no? >> Yes.
[45:49] >> Great. What I love about Tailwind, they have great documentation.
[45:52] You got that quick search in the upper left. Let's go look at font size and see how to bump that font size up.
[46:00] >> Yay. >> There you have it.
[46:07] They have different font sizes. You can make it Excel or something,
[46:13] have it be relative, or you could choose a specific size.
[46:19] I think there's some pixel-based ones. How much bigger do we want our h1 titles here,
[46:24] like the page header title? >> It didn't load because we're doing stuff.
[46:32] >> Let's go back. We can fix that real quick. Let's just go back to the Gitpod.
[46:38] I think you need to have the quotes after a class name equals. Exactly. Perfect.
[46:47] >> Yay. I would say it needs to be probably about 20, maybe 24. >> That's perfect. Let's go back to Tailwind font size there.
[47:03] They give you pixel indicators. That's going to be text-to-Excel.
[47:09] You should be able to just copy that class name there, add it in on Gitpod,
[47:16] give the page a refresh, and boom, we've bumped up our font size.
[47:21] >> There we go. >> Then?
[47:32] >> What else do we want to make it? What other styles come to mind?
[47:38] >> Font weight. >> Would I have to do another class for that,
[47:46] or can I use this in the same class? >> You can use it in the same class name.
[47:52] The class name here works just like class with normal HTML and CSS where you can specify multiple classes.
[48:02] >> Is that like a comma and then putting it in the same? >> It's space delineated.
[48:11] If you just give it a space, that's how they separate the stuff out. There we go.
[48:17] >> Yay. Then I would say the last thing that I want to do is,
[48:31] you said that if I just want it to have more space around it, what is that called again?
[48:43] >> That's going to be margin. If you just want more space around it,
[48:48] we're not using a background color or something here, we're trying to separate elements, that's margin.
[48:54] >> Add a margin to all sides. >> Taylor makes it easy if you just want
[49:06] vertical margins or horizontal or add margins everywhere. If you scroll up, it'll give you
[49:14] the what the different sizes mean as well. These are the examples here.
[49:20] >> I probably want M2 or M4. >> Yeah, let's try it out, see how it looks.
[49:29] >> This is so exciting being able to actually see this happen. >> Four.
[49:39] >> Oh, yay. >> Yay, there we go.
[49:52] >> This is way too exciting. >> Yeah. I'm wondering just for testing purposes,
[49:57] it might be nice if we could get the hello beautiful human to line up on that left-hand side with our mission,
[50:06] and maybe flip the video, stack the our mission and the photo above the video,
[50:11] just move those around so that we can check out some of that alignment.
[50:15] Let's start with switching the content sections that we have for
[50:22] the video and the side-by-side there. Let's just flip those on Gitpod.
[50:28] >> No, we can't change it to hello hideous human, Anthony. >> No.
[50:34] >> No, that's not something I say. >> No.
[50:37] >> Only like really mean evil people. But even then, I struggle with it.
[50:44] Documentation is the real MVP. We are going to take this and do it above this.
[51:06] >> You'll still want it in that simple layout though. The simple layout is wrapping everything.
[51:12] That's where that layout defines our header menu and our footer and stuff.
[51:18] >> Perfect. >> Then I want to see how,
[51:24] wait, go here. No, side-by-side.
[51:43] >> Justify center, space 8x. Is that how you did it to match our mission?
[51:55] >> Yeah. It's weird. Basically, the outer layer there,
[52:01] the flex box is like, where am I putting these elements?
[52:05] Because I could put them anywhere. We're saying, hey, put them together in the center.
[52:10] For that div, that's where we're specifying how big they could be.
[52:19] We might want to think about how our layout works here. >> I'm writing myself notes too
[52:35] because I know we're going to run out of time soon, and I'm like, but I'm finally getting it.
[52:40] I want to be able to do this later. Who knows? I'm probably going to
[52:43] live stream at some point tomorrow now. Yes, y'all, I'm writing on paper.
[52:53] It's a thing that people used to do. >> That's okay. We use Excel a lot.
[53:04] A lot. It's a thing people used to do back in the '80s and '90s, I know.
[53:10] There's not an app for what we do yet because we're trying to build
[53:13] the app for what we do. Do you know what I'm saying? >> Yeah. Then would it be a margin,
[53:21] just because I'm taking notes for myself to work on it later, would it be a margin around this section or would that?
[53:29] >> Yeah. I think if you want to separate, you see how that photo runs into the YouTube video?
[53:35] >> Yeah. >> That to me says it's a layout issue.
[53:38] It's not the content that needs to deal with that, it's each section needs to provide
[53:44] some space between itself and the previous sections. I would look at adding margin to the sections.
[53:51] You might not need side margin, maybe you just need vertical margin.
[53:56] >> Exactly. >> I think the cool thing is, yes,
[54:02] I'm writing it here, but I can actually put these notes in my issue.
[54:08] >> Yeah, that's a great point. >> That way I remember what I'm working on next.
[54:11] >> I'd recommend using GitHub's checkbox feature, so it can be like add margin between sections,
[54:16] and that way you can check it off when it's done to communicate to other people,
[54:21] your progress as you're working your way through it. >> Because I think this would be really cool.
[54:28] I guess just now that I'm starting to get the hang of it, the other part that you wanted,
[54:34] and I just want to make sure I understand it because it probably is in the text,
[54:37] but I want to make sure I understand it, is you wanted two sections,
[54:46] like our mission where the text is on the left, and then do another section that says the text is on the right,
[54:52] so that way they have either choice? >> Yeah, that's going to get
[54:57] interesting because we have a few options. We could say, here's a section with
[55:02] a single piece of content and here's a setting. Is it left, center, right?
[55:08] We could also say we want those as explicit sections. I think we got some options there.
[55:16] That might get more into when we refactor this out into reusable components.
[55:20] For now, I would say just set up examples. We just want lots of different examples with
[55:26] different pieces of content and different layouts to know what we're looking at for our options.
[55:32] When we refactor it, we can make some architectural decisions.
[55:36] Do we want to have this be a parameter you're feeding into the component,
[55:41] or is this like a core piece of the component itself? >> Interesting. Just to
[55:50] check if it's possible before I go down this rabbit hole, I think that's the other thing,
[55:54] is if I wanted to change the header or change the class on here, I would just make them two different areas.
[56:04] This one is an h1 with a class, and then I would do a paragraph with a class.
[56:09] >> Yes. The interesting thing for that text is it's from markdown,
[56:13] so you're not really going to be able to change that. We've actually started to solve
[56:19] this issue on a different branch. Folks, this is exactly why we do draft pull requests.
[56:24] I found a library to apply tailwind styles automatically to markdown content.
[56:31] Instead of having to go in, because you can see right there on line 35,
[56:36] we don't have access to all of that markdown content. It's not written out as different HTML elements.
[56:44] Be very complicated for us to go in and change how the markdown gets
[56:49] rendered and add class names based on different components. This tailwind extension does it for us.
[56:59] That might be something that we want to actually merge some of that work into your branch before,
[57:06] or maybe get it into Saga and then pull it back to your branch. But what I'll say for now is don't worry too much about
[57:13] the markdown content block specifically. It's just good that we're actually rendering the markdown for now.
[57:20] You can worry about how is it spaced compared to other blocks, like that side-by-side, does it need more space?
[57:27] Do you maybe want to have a vertical line between them, providing some more visual separation?
[57:32] I think there's a lot of different stylistic directions you can go in. On the layout side,
[57:38] just don't go down a rabbit hole and I'm trying to style the markdown content,
[57:42] because that's going to be pretty tricky. It was even too tricky for me.
[57:45] I'm like, "Nope, someone solve this problem, I'm going to include their stuff."
[57:48] >> All right. I totally dig this. This is a really cool project
[57:54] and I'm excited that it's one of my first projects. Because it's definitely stuff that I've talked to
[58:02] a couple of back-end developers and I'm like, I like what they do and I'm curious about it.
[58:09] But I'm like, I like front-end development because I'm like, "Look, it looks pretty. I can make it look pretty.
[58:13] I can go fix it in it." Where back-end in my mind at least I'm like,
[58:18] "Oh, so they're going to make it work, spit out the data, everything like that."
[58:25] It's definitely, I like learning both. >> Let's not forget,
[58:30] you want to make a quick commit and push it, so we don't lose your progress, right?
[58:35] >> Yes. Thank you for the reminder. >> Okay. I'm trying to think if I remember.
[58:50] I don't, because it was like we did it out of a different order than I remember.
[58:57] >> Let's walk through the proper order and then this is going to be a good one to write down,
[59:01] because this is like a very regular, lots of little commits and little checkpoints.
[59:06] >> Yes. Anthony, if you are still watching and listening, FYI, I did do my read me yesterday for more Python.
[59:18] I just forgot to update my read me, so I can do that here.
[59:22] >> Slowly. It is, is it git command? >> Let's not worry about the git commands,
[59:45] because those are actually fairly confusing. I think people have a fair criticism
[59:49] of git strange incantations. What's the first thing that we want to do here?
[59:54] There's going to be a series of steps we need to take to get this pushed on to your work in progress branch.
[60:01] Maybe you want to check what changes have happened so far, especially if you're working in multiple files and folders.
[60:10] What am I actually looking at here compared to when I started? >> That's what I like to do in
[60:19] case I accidentally change something else, I don't want to include yet or something.
[60:23] A git space status, that just gives you a status check like what's going on.
[60:29] We can see the branch we're on makes sense. We've changed one file, also makes sense.
[60:36] Now we need to take a look at our changes. We need to add those changes in.
[60:42] You don't have to commit everything at once. Oftentimes, I might be changing a configuration file.
[60:48] Let me go commit that and then continue my work and do a larger commit later.
[60:54] Now we can do git add. Exactly.
[60:58] >> Well, on this one, because I only did it in here,
[61:04] I could do git commit all, which is that dash all?
[61:09] >> That's true. That's true. But I think it's good to just follow the process.
[61:17] Don't worry about, that's one of the reasons gets confusing as it gives you multiple ways to do the same thing.
[61:23] I would, until you get real comfortable with the command line stuff here,
[61:28] just try to follow git status, git add, get that flow down first.
[61:34] In this case, you need to specify the files. Yeah. You can say git add dot,
[61:41] which is like add everything, all the changes. You can also, if you wanted to put just source/pages/page.template,
[61:51] you can specify the specific files. You can run add multiple times.
[61:57] If we had 10 files that were changed, you could say add all the files in this folder,
[62:01] and then add that configuration file, and don't add these ones.
[62:06] >> If I wanted to, just for my own clarification,
[62:10] I could do git add and then /source, and I would do everything in that?
[62:17] >> Not a /, just src, because this is relative just like the file directory.
[62:24] That'd be everything in src. If you did src/pages,
[62:27] that'd only be stuff in pages. If you did src/pages/page-template.tsx,
[62:35] that would just be that one file. >> Cool. Then so it's all been added.
[62:45] >> Been added. Yeah. Let's run git status again, so we can actually see that.
[62:49] You can confirm, never hurts running a git status here. >> Yeah.
[62:54] >> Cool. Now we're ready to make our commit. We've made a change,
[62:59] we've added that change, it's set up, good to go.
[63:01] Now we can commit it. >> Yeah.
[63:05] >> Okay. Then it's git commit, and then is it this wiggly M?
[63:14] >> Yeah, it's just a dash, not necessarily, just dash M.
[63:18] >> Then changed. >> You'll want quotes.
[63:24] You'll want quotes. If you remember, we use something called conventional commits,
[63:29] which is really just has tags. In this case, you've made progress,
[63:33] you want to do feats colon space, and then write your message there.
[63:38] Yeah. I think we do a lowercase feet without the S, but I don't actually care about that that much.
[63:45] >> It's good to know and it's practice. Feet, header, sizing, and moving sections.
[64:02] All right, there. >> Great.
[64:07] >> Yay. >> That's perfect. Now the last thing,
[64:10] so that ran some automated commands to auto-format things. We still haven't sent it to the server,
[64:17] so that's the really important last step. Do you remember how to do that?
[64:21] >> No, because I thought the git commit did it. >> The git commit, it's your save point locally.
[64:31] So all of that was like, "Hey, let me save my progress here locally."
[64:35] The last thing you want to do is do a git push, and that'll share those changes up.
[64:41] So just to recap for the audience, we do git status, git add,
[64:46] do another git status if you want, git commit, and then git push.
[64:52] Now you see right there, now it sends it up to the ticket hub.
[64:59] >> Yeah. >> Sweet. This was definitely insightful,
[65:04] and I'm excited to at least start working on this and reading through it
[65:08] now that I'm starting to get the hang of it. Lots more to do with Distribute Aid.
[65:17] Once again, thank you for being on the show. If we have this spare time next week,
[65:21] I may be hitting you guys up again. >> You should. Yeah. We're doing a couple of fun things.
[65:26] Y'all check out Distribute Aid's OSS Thursday stream later this week.
[65:31] Next Tuesday, I'm going to host a Code Jam. We're not going to do that live,
[65:35] but I have a Zoom link if anyone's interested in just hanging out,
[65:39] hacking on Distribute Aid, sort of office hours set up.
[65:42] Maybe you get a group of us on there. Then we have another live stream on Thursday.
[65:47] Jen, please, you're welcome anytime you want to come on our stream,
[65:51] and I'd be happy to keep working with you here, making some progress.
[65:55] In the meantime, feel free to hack away on your own time. I think you're getting the hang of it.
[65:59] You can get the style done, and then maybe the next time we look at it,
[66:02] we can look at refactoring those out into components, separating them from the page so we
[66:08] can embed a YouTube video anywhere we want. >> Yes. Thank you again,
[66:14] and looking forward to getting more movement on this. Talk to you soon, Taylor, and thank you all of
[66:20] the homies, beautiful humans, hood mob. >> Friends.
[66:26] >> Friends that have joined. >> Cool.

