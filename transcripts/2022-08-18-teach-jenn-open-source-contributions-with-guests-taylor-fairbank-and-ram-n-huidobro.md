---
showLink: "https://www.youtube.com/watch?v=DEPtUQibCAA"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-open-source-contributions-with-guests-taylor-fairbank-and-ram-n-huidobro"
title: "Teach Jenn Open-Source Contributions with guests Taylor Fairbank and Ramón Huidobro"
publishDate: "2022-08-18"
coverImage: "https://i.ytimg.com/vi/DEPtUQibCAA/maxresdefault.jpg"
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

[00:00] We'll have her in the background. Hello, beautiful humans.
[00:04] Thank you for joining another day of Teach Gen Tech. We have, yes, me talking about my dog in the background
[00:12] and also Taylor and Ramon. This is Ramon's third time being on the show,
[00:18] which is exciting. And this time he brought a guest with him, Taylor.
[00:24] And please introduce yourselves and what will be, le, le, words.
[00:31] What will we be learning today? What are you teaching today and what am I learning?
[00:38] Why don't you go first, Taylor? Okay, hey everybody.
[00:43] I'm Taylor, I'm the Operations Director at DistributeAid. I'm sure we'll talk about DistributeAid in a minute.
[00:50] But yeah, kind of went to, got into tech in high school, did comp sci in college, dropped out of college,
[00:57] did the tech startup thing and loved the early stage work building,
[01:01] hated the, you know, kind of money focus on startups in the Valley.
[01:05] So now I bounce between Pittsburgh and Belgrade, Serbia, where I'm currently at doing this aid work
[01:11] and building some tech alongside it. Very cool, and yes, I have questions.
[01:17] And yes, I found my glasses, Sky. I'm very excited because I was running around very blind.
[01:26] And Ramon, who are you and what are you going to be teaching us?
[01:32] - Well, I'm laughing because this is the, like, it's been a long time.
[01:36] I've been hosting a lot of streams this week and I went to click on Kai's comment
[01:43] and I realized I couldn't highlight it because I'm not the host.
[01:46] And I was like, oh yeah, I'm not hosting. - Oh, but this is fun.
[01:50] Like I didn't know it would move all of our videos to see Kai's comment.
[01:56] Yes, I did find my glasses. I found a pair.
[01:59] I have multiple. That is the one thing I didn't get to tell you, Kai,
[02:02] is I have multiple pairs of glasses that I lose. - Yes, hi everybody.
[02:09] My name is Ramon. I'm tuning in from Vienna in Austria.
[02:13] I'm a developer advocate and developer educator. And I'm here to help out with teaching Jen
[02:22] a little bit of open source contribution, a little bit of, like I was telling her earlier,
[02:29] we're going to be doing, what is it? Like, and not to scare anybody,
[02:34] but we're going to be doing TypeScript, Gatsby, GraphQL, Tailwind, the whole mess of stuff today.
[02:42] - Yeah, plus throw in Gitpod, little bit of CodeSea, you know, some of those dev tools.
[02:47] - And y'all, I just want to let you know that I asked them to do this.
[02:55] It was like, hey, this could be a really fun idea. So I know I signed up for something difficult,
[03:00] but I think it's really fun in the fact that learning very, very complex items
[03:09] and then breaking it down afterwards is something that I found is a learning style
[03:14] that helps me a lot, because then I know why I'm learning these bare basics,
[03:18] where if I just learned the bare basics first, I'm not great at remembering them either
[03:25] if I don't know where they go. - It's like a learn by doing
[03:29] and having a real world application. You're like, oh, this is why it's important.
[03:33] It makes a lot of sense. - Exactly, exactly.
[03:35] And thank you for joining Daylight Turkey and Noel. Okay, Daylight Turkey, that's just kind of fun
[03:43] because I don't know your name, so I'm actually saying your username and that's awesome.
[03:50] And also thank you everyone for joining because I don't know if you have this
[03:56] when y'all live stream, but I have this like notification
[04:00] that I have to have five people talking at the same time in the chat.
[04:06] And it's been driving me insane that I have that notification.
[04:09] - Wait, what is that notification? - On Twitch.
[04:15] Okay, hold on, hold on. - Like a merit badge on their platform or something?
[04:20] - Yes. - Oh. - And it drives me nuts
[04:24] 'cause I'm like, we've had that many people. I don't know why it, you know, like, look at this.
[04:31] It just says four. You have to have five people chatting at the same time.
[04:35] And I'm like, just go away 'cause you can't clear it either.
[04:39] It's just stuck there. So who knows what the next thing
[04:44] I'm gonna be really annoyed and stuck at. But that is, so I appreciate everyone joining.
[04:50] And thank you, Finn, for joining as well. Nice one, Ramon.
[04:56] I dig it, I dig it. All right.
[05:01] - If we need chatters, we can get more folks in there. In fact, I'm gonna go ahead and retweet
[05:05] and tell people we're live. But yes, like just to preface what we're doing here
[05:10] because not, it's like not to, not to, you know, override what we're doing here
[05:17] with Teach Gen Tech. But usually at this time of week,
[05:20] Taylor and I are streaming through Distribute Aid, doing something we call OSS or Open Source Thursdays.
[05:28] So this is kind of a, is this like a crossover episode, a collab?
[05:32] I don't know what to call it. - I love it, yeah.
[05:34] Crossover episode, right? Like, it's so fun. - I'll come on your guys' show
[05:39] at some point. It's gonna be awesome.
[05:41] - Yeah, anytime. - Awesome.
[05:44] - No, we have a ton of fun. And I think our, you know, our style is perfect.
[05:47] Like you're trying to learn tech. We use a lot of ensemble programming techniques.
[05:51] So anyone in the audience, we get stuck a lot. Like you'll see me and Ramon Googling for things.
[05:57] You got an answer. If you wanna like look at the documentation with us
[06:00] and point us in the right direction, please let us know.
[06:03] 'Cause I've been doing this for a while, but you know, still always running into new problems,
[06:08] new challenges, forgetting the command name or the style name or something.
[06:13] Yeah. - Noelle and I were doing that last week
[06:16] and it was a lot of fun. So that's a big reason that I was like,
[06:20] all right, we gotta do this. And now I am curious, so what is DistributeAid?
[06:28] - Oh yeah, I get to do my pitch. So DistributeAid, I think at this point
[06:34] is the world's largest grassroots mutual aid supply chain, right?
[06:41] So like supply chains are really big. They deliver trillions of dollars worth of goods.
[06:46] So, you know, the grassroots, we focus on community-based organizations.
[06:52] Most of our partners are run by volunteers. We're also an all volunteer team, you know,
[06:57] with a kind of cost of living stipend for our full-time members, right?
[07:03] And mutual aid, it's this idea, it's really gained a lot of popularity,
[07:08] especially in the US, like during COVID times, kind of the year of 2015,
[07:13] responding to the so-called refugee crisis. It's this idea that we're helping people out,
[07:20] but it's not like charity. We're not just sending resources or sending supplies,
[07:26] you know, we're really trying to look at what are the core problems and challenges
[07:30] people are facing? And also like, what do we get out of this work, you know?
[07:34] So this mentality that we're in it together, you know, with the people that we're supporting
[07:39] and we're benefiting by supporting them. So yeah, we do lots of logistics.
[07:46] We also do some open source tech to help power that logistics.
[07:50] And that means import and export. We schedule trucks and shipping containers.
[07:55] We deal with customs. We work with our community partners
[08:00] to do needs assessments, which is powered by one of our other open source projects.
[08:05] I think we tracked 74 million needed items over the past year or so.
[08:11] And then work with the collection side. So that'd be community groups, just gathering aid,
[08:18] secondhand clothing, you know, donated tents, kind of, you know, hygiene items purchased
[08:24] from the local grocery store. Yeah, to gather all that aid
[08:28] and really help these smaller community groups access the very large global supply chain
[08:34] to get the aid to our smaller frontline partners and ultimately get it in the hands of the people.
[08:39] It's really important and rewarding work. We often work alongside much larger organizations
[08:46] like the Red Cross. I think recently I was working with the US government
[08:52] at Fort Pickett, one of the Afghan safe havens running the supply chain there for a Ukraine response.
[08:58] There are obviously a ton of very large actors, but our grassroots partners are really able
[09:02] to get in there and fill the gaps, right? And take care of people that are in, you know,
[09:08] less concentrated areas that are overlooked, that might be, you know, marginalized in some way
[09:15] in these situations, right? And yeah, and we all learn from it
[09:21] and everyone kind of grows and benefits together. So we're really proud over the past year,
[09:26] as you can see on the screen, July, 2021 to June, 2022, we shipped the equivalent of $14.7 million worth of aid.
[09:36] It's translated to kind of the USA GDP context. We only had about a $200,000 budget, right?
[09:44] We're still an all volunteer team. So that meant, you know, Jen, imagine I hand you a dollar
[09:48] and you walk out of Walmart with $87 worth of stuff. Like that's our impact ratio.
[09:54] We're multiplying that by 87, you know, saving groups money,
[09:58] helping them efficiently access this logistics, you know, making sure that the aid set is needed.
[10:04] It's not trash. It's not something that's gonna sit
[10:06] in the warehouse gathering dust. So we're just thrilled to be what we're doing here.
[10:12] And we really see the tech side. That's our long-term play, right?
[10:17] Open source, you know, it takes a while to build tech products.
[10:21] We had to build a whole supply chain in order to kind of normalize the operations
[10:26] to a point where they're repeatable enough that we could build tech on top of it.
[10:31] And it's not about us. Like I'd love to retire at some point.
[10:36] So by building this sort of open source tech, we can empower anybody to do the sort of work that we do,
[10:43] right, really spread that knowledge and spread those processes out
[10:46] throughout our entire community. - First off, that is so dope.
[10:52] Finn said, "That's incredible." And Noelle said, "Great stuff."
[10:59] Agreed, agreed. And hello, Ben, officially.
[11:03] Now, first off, that is like just kind of bananas thinking about it and the impact.
[11:11] And also so many questions for another time because I don't understand as much as I would like to
[11:19] for supply chain and like what goes into it, but something that you're actually, Ramon,
[11:29] you're on this page. So I think this is perfect.
[11:31] Like you have donate here, yet you talked about it also being open source
[11:36] and like that's another way we can like donate our time by helping on that.
[11:42] So where do people like go find this information? Is it on the donate page?
[11:47] Like go donate your time as a coder or is like, where do you have that stuff?
[11:52] - That is a really great question. One of the problems with our website
[11:57] is that we kind of would update it and then get really busy doing the aid stuff.
[12:01] We're a very like action oriented team. So it all gets sucked into like responses and things
[12:05] and it would not get updated for a year, right? And then we'd update it again
[12:09] and then it would not get updated for a year. So I think a lot of our code stuff,
[12:13] if you go to any one of our GitHub repos or if you go to our main GitHub page,
[12:18] we have lots of ways for people to tap in there. But that's a great point that we should put more avenues,
[12:25] you know, folks visit our website and like direct people to contribute to our code bases.
[12:31] So yeah, I think that's like, you know, on GitHub, you know, on places that tech folks
[12:37] are like tapped into like Twitter, we really try to make it easy for people to get involved
[12:43] and absolutely love it when they do. You're absolutely right, like make a contribution
[12:47] to one of our open source repos, 10 bucks a month helps deliver $10,000 of aid.
[12:51] Like it doesn't matter, right? We just wanna get people involved in these movements
[12:56] and helping others. - That, words, like I think a lot of people
[13:03] that are currently in the code space, you know, they'll know to look at GitHub and stuff,
[13:14] but if you go to the donate page itself, it does show Open Collective.
[13:23] So I do just wanna point that out. So that way we know that there is another different ways
[13:30] to donate time and money. That is, and especially with being unemployed for so long,
[13:37] I'm excited that there is a way to donate time. - Yeah.
[13:41] - And learn to code and work on doing this. So that being said, yes, I have tons of curiosity questions,
[13:49] but they have nothing to do with the project itself. Where do we get started today?
[13:58] And Ramon, are you gonna drive for a majority of it or you want me to drive?
[14:02] - Well, I would love to, as always, make this a Ensembl programming opportunity.
[14:11] Jen, if you're feeling cool with it, we could have you drive. Taylor and I would help navigate
[14:18] and everybody in the chat, and I mean everybody, you are invited to be part of the Ensembl.
[14:24] That means Jen will be doing the actual hands-on coding. Taylor and I will be guiding, asking questions,
[14:33] answering questions, and that sort of thing. Everybody else in the audience, you are the Ensembl,
[14:38] which means you're asking questions, you're looking up stuff in the documentation,
[14:45] you are helping us with CSS stuff and with Tailwind and stuff 'cause stuff's gonna come up and it'll be totally fine.
[14:56] But yeah, today, our big overarching, arching, I'm gonna go with arching, our big overarching goal
[15:06] is to bring and onboard Jen as a contributor to DistributeAid, and in order to do that,
[15:16] we'll get you on our GitHub. So here's a question for you, Taylor.
[15:24] Do we have a link to GitHub on the main page? Should it be there?
[15:29] - We definitely should, like in the footer or something at least, and that might be a cool thing
[15:33] we can add right here on the stream. - I think so.
[15:36] - Yeah, 'cause we already have the icons there, so it makes a lot of sense to me.
[15:41] - I agree, and I do wanna say, Ben, I did tell them that you taught me how to submit my first PR.
[15:49] So they do know that I have done it and that you taught me 'cause I'm also nervous to do it again
[15:58] because it was a lot of like peeking at my notes and going, what am I doing again?
[16:03] Okay, but I'm excited because it's like, practice is the only way to get it to go through.
[16:09] And also, I get that y'all already have a README file. I'm gonna be creating my own README
[16:16] because that is my way of practicing my READMEs as well as it'll make for great blog content
[16:26] at some point, when I'm not live streaming or Twitter spacing or going to the office.
[16:32] So, all right. - No, that sounds great.
[16:37] Yeah, I think practical for stuff to get started. Let's go to the DistributeAid GitHub
[16:42] and we wanna choose the DistributeAid.org. Yeah, I think it's not, oh, there we go.
[16:49] Yep. - No, no. - No. - Oh, there's a typo.
[16:52] - That's so wrong. - It says there's a typo, there's a missing S in distribute.
[16:57] - Oh, no, there we go. See, y'all, you can be an amazing organization
[17:01] and still mess up the good stuff. - But that means that, and I'm just curious.
[17:07] So, I'm gonna open this actually in another tab. I wanna see if I remember how to do this.
[17:13] This actually is a great, would this be, this site is open to the public.
[17:24] - OpenCollective? - Yeah, OpenCollective is a really cool
[17:28] fiscal hosting platform. And so, that's how we have charity status in the US
[17:33] is we're fiscally hosted by OpenCollective. So, we can accept donations from people
[17:37] like monetary donations on the US. - So, where would you put a issue
[17:45] to remind you to go fix that? - That's a good question.
[17:52] Yeah, I think since it's probably not tied to one of our coding repos,
[17:58] I'm gonna file it right here and also take some notes. We bring that up in our once a week admin meeting.
[18:04] So, that's kind of our chance, our hour every week to say, hey, here's the things we can improve upon
[18:08] or what are we working on this week? And we use Notion to track that.
[18:12] - I love Notion. - Notion's great.
[18:16] - All right, so I need a-- - I'm gonna add a quick note right now to our Notion.
[18:21] - I didn't know you could follow an organization. That's fascinating.
[18:25] - Well, I think I do because, let me go back here, 'cause I follow Open Sauce.
[18:38] - Oh, yeah, cool. - I think, I don't know.
[18:40] Let's see if I actually followed all of it or if I just followed that one.
[18:46] Oh, yeah. - It says there, unfollow. Nice.
[18:48] - Sweet. All right, Kai had a good question.
[18:55] They were gonna ask where content for the website type issues would come up
[19:01] because that's something where I could easily contribute. - Taylor, you're muted.
[19:09] - Classic, it happens like at least every other Zoom call. No, I really appreciate that, Ty.
[19:18] Definitely reach out if you wanna ship me a message at borderlessdev, so I have your, that's on Twitter,
[19:25] or hello@distributed.org for email. Love to connect, get you involved.
[19:31] So that link from Open Collective, 'cause that was on the Open Collective side.
[19:34] That's not a good thing. But if there's actual stuff with the website,
[19:38] like adding a GitHub icon and being able to click and access our GitHub to the footer of the webpage
[19:45] or on the donate page, like other ways to contribute, that would be the perfect thing to add
[19:52] to our landing site repository. So Jen, if you want to go to Distribute Aid there,
[20:00] and I think if you scroll down in the overview, it shows our active projects,
[20:05] or if you click on the list of repos we have, yeah, that should be the link right there.
[20:13] - Cool, so project seeking contributions. Yay.
[20:22] - Perfect, and that's the distributed.org project for our landing site.
[20:26] So this will be the place. If anyone wants to get involved,
[20:29] we have some Help Wanted issues open on the issues tab. And please, please, please do file issues
[20:36] if you notice anything on our site that can be improved or content you'd like to see, things like that.
[20:41] - I do have something, if I may. Jen, could I ask you to maybe enlarge
[20:46] the font size a little, please? - Oh yeah, for sure.
[20:49] I like how it like did that for this one, and then I don't realize when it doesn't do it
[20:53] for like all pages. - Yeah, totally fair.
[20:56] - All right. - Much better, thank you.
[20:59] - Yay. - If anybody watching wants it a little bit larger,
[21:01] just let us know, please. - Yes, definitely.
[21:04] And then for us today, are we gonna be looking at issues or?
[21:11] - Yep, we got an issue specked out just for you, Jen. - Yay.
[21:17] - Yep, so the one I created this afternoon is that first one there, number 523,
[21:23] set up generic pages and content components. And I wrote a whole bunch.
[21:30] I might have overdone it on the description. - Wow.
[21:34] - But yeah, I think the idea is that we, Ramon and I on our stream have been working
[21:39] on a lot of data-driven pages. So things like our regions pages,
[21:44] where we can mop up like a regions template in our content management system.
[21:49] And then the admin team can go add the dozen regions that we should need to.
[21:53] And then all of those pages show up and they have the same format, right?
[21:57] Region names, sub regions, current events, things like that. We also have a ton of pages that are kind of unique.
[22:06] The about us page or the how to contribute code page or some guide on exporting aid from the UK, right?
[22:15] And so they don't follow a consistent content format. What we'd like to do today is kind of start from the front
[22:23] and work our way backwards, right? Which means, you know,
[22:26] start by just hard coding some HTML onto a page and then refactor that until we end up
[22:33] with a kind of generic page template and these different content blocks.
[22:39] And what that will allow our admin team to do is create a page and then specify, okay,
[22:44] I wanna start it off and here's the opening paragraph. And then here's a paragraph with an image next to it.
[22:50] And then here's a YouTube embed and it'll give them the flexibility, you know,
[22:55] for any one of these pages, it's not all gonna look the same.
[22:58] They need different content. Our admin and ops people can choose that content
[23:02] and they can get these pages up and running without needing to wait on the dev,
[23:06] which really is a great way to empower non-technical contributors to your technical projects, right?
[23:13] Just remove barriers and set things up in a flexible manner. So they don't have to wait for devs
[23:20] who are not acting as gatekeepers to getting changes live. So a pretty important issue, definitely a challenge,
[23:27] but I think the three of us are up to it. - I will say, so for this,
[23:33] something that I learned earlier this week was like commenting in here and saying,
[23:39] "Hey, can I take this?" So that way we're assigned.
[23:43] So, okay, yes, yes. I saw happy dances, so we're-
[23:47] - Happy dance means go for it. In fact, what I can do is assign it to you.
[23:54] - Sweet, I commented. That was fun.
[23:57] - If you stay there, if you stay there, 'cause I think GitHub does this automatically,
[24:02] I will say, oh, wait, I'm not logged in. Give me one second.
[24:05] (laughing) Give me one second.
[24:08] Wrong, too many browser windows. - Absolutely, thank you for your help.
[24:14] - Y'all, it's getting a bit choppy. It's getting a bit choppy for me.
[24:19] I'm just gonna switch from my wifi to tethering through my mobile phone.
[24:23] So if I drop out for half a sec, I'll be right back. - No worries, no worries.
[24:28] I can hold down the fort. - Keep it rolling. - Yeah, yeah.
[24:31] So I'm gonna comment now. Absolutely, thank you for your help, which should, hey.
[24:37] - Yay. - So if you stay at the bottom real quick.
[24:42] - Okay. - Yeah, let's, what's it, teach gen tech.
[24:50] See? Oh, wait, do I need to like?
[24:57] - Oh, yay, okay. - So let's take a second and talk about
[25:02] like assigning issues on GitHub. Because like this can sometimes, you know,
[25:06] in a sense, like bring on a bit of pressure, right? It's like, oh my gosh, do I have,
[25:09] am I like fully responsible for this? And what if I draw, like, what if I get busy?
[25:13] What if I get a new job and I, you know, need to fully focus on this for a few weeks?
[25:18] What happens? Of course, this depends on the etiquette and like usual,
[25:26] you know, every day goings on at an open source project. But usually, usually this means
[25:35] that if somebody's coming in and being like, oh, you know, I'd like to work on this.
[25:38] And you see that they assigned it to themselves, like, I don't know, like month and a half ago,
[25:42] and they're not really working on it. Nothing's stopping them from coming in and being like,
[25:46] hey, Jen, are you still working on this? 'Cause if not, I'll happily take over.
[25:49] And then usually you'll respond and say like, oh, you know what, I did get rather busy.
[25:53] Like, do you mind taking over? And that's totally fine.
[25:56] What I'm getting at is, don't stress about having this assigned to you,
[25:59] and then maybe you can't follow up on it later. There is time, maybe we can get back on it later.
[26:04] Like, this is flexible. - I'm like, so does that mean we're doing it
[26:09] like on your stream one of these days, like to finish it out?
[26:13] - However you prefer. - Worst case. - We can stream it, we can come back to it.
[26:17] We can do it, you know, on our own time. Like the door is open.
[26:21] - Yeah, yeah, I think, you know, just being really flexible
[26:25] and communicating well with each other. And like, it's very understandable.
[26:28] Like everyone goes through busy periods, you know, everyone like gets excited about an issue,
[26:34] and then it's kind of like, you need someone to help you cross that finish line.
[26:38] On the flip side, Jen, you might fall in love with the coding we're doing today
[26:43] and really like distribute aid and get this PR up, and then want to assign yourself the next issue, right?
[26:48] - I'm digging it, I'm digging it. All right, so now that I have it assigned,
[26:54] if I remember correctly, I need to fork it and then clone it on my computer.
[27:01] - Well, you will be forking it, but we're gonna be trying something new today.
[27:05] So go ahead and fork it. Well, new, we've done it before, but like new, sorry.
[27:10] - Oh, I'm wondering if, nevermind. I'm usually not used to forking things
[27:16] because I'm just like on the, I can just, yeah. - You gotta handle the forking here.
[27:22] I'm not very familiar with forking. - Oh, you're good.
[27:24] I think the reason we want to fork, Taylor, is so that Jen can push commits.
[27:31] - Hmm, gotcha. That's cool.
[27:33] I could also just add her to our devs list. - If you want to do that, we can do that too.
[27:38] In fact, actually, do we want to add Jen as a contributor first thing?
[27:43] - I mean, that seems like an easy way to go about it. It depends.
[27:48] Jen, do you want to fork? Or do you just want to like join the Distribute Aid team
[27:51] on GitHub and so you can push directly to the repo? - I am down to join as a dev,
[27:58] as long as when I need to do this kind of stuff on other open source, y'all will help me through it
[28:06] if I don't remember. - Yes, absolutely. - Of course.
[28:09] - Okay, so that means I need to go back here, no. - If you move your mouse a little bit lower, you'll see.
[28:18] - Oh, my face wasn't planning on that one, but. - I think what you can do is go back twice.
[28:29] Then go, see where it says forked from distributeaiddistributeaid.org?
[28:39] - Oh, okay. Yeah, yeah, yeah.
[28:41] - Yeah, that's it. - Yay, I'm back. - Yeah, and then as soon as Taylor gives us,
[28:46] actually, we don't need the get go from, we don't need the word from Taylor
[28:49] because what we can do, Jen, is start you off, but with something a little bit new.
[28:55] 'Cause a lot of projects you can contribute, say, by cloning to your computer, which is all well and good
[29:02] but what Taylor and I usually do on stream is we actually use a tool that lets us do
[29:06] live collaborative coding called Gitpod. And it's something we'd love to try out with you today.
[29:18] So in order to do that, what you got to do is scroll down a little bit,
[29:24] down to the readme. - I was like, I see a Gitpod.
[29:30] - No, you're good. So scroll down to the readme.
[29:33] Yeah. - And I have added Jen to our dev team on GitHub.
[29:39] Yep, with great power comes great responsibility and don't worry.
[29:43] I don't think you can break anything. That's irreversible.
[29:46] - I was going to say, as long as you guys can fix anything, if I break it, if I do break it.
[29:51] - No. - For what it's worth, Jen, we break stuff all the time.
[29:55] - All the time. - Okay, I dig it, I dig it.
[29:59] - So you're going to see a button a little bit higher up that says open in Gitpod.
[30:04] Let's go ahead and give that a click. And this is going to get you logged into Gitpod,
[30:12] which will ask you to sign in, like link it to your GitHub account.
[30:16] And what's going to happen is it'll let you, you want to go with VS Code browser.
[30:25] This is to pick your editor. And what this is going to do is spin up
[30:30] a development environment on your browser, as well as a coding editor.
[30:38] It is as if VS Code is running live on your browser. - Interesting, okay.
[30:47] - Along with a terminal. - Interesting.
[30:52] - We've set it up so it does all of the, all of the like NPM install, NPM startup,
[30:59] the local server automatically. So what you'll see, well, first off,
[31:05] would you mind making it a touch bigger, please? I'd say that's a good size.
[31:14] Again, folks, if it's too, if it's too small, just let us know.
[31:19] And I think you can, yeah, you can close those. Yeah, now you're going to see on the right hand side,
[31:27] there's these like little terminal signs on the right most column.
[31:34] You see, there's these two, you're good. - My setup is my laptop covers the corner.
[31:40] So I'm like, hold on, I need to figure that part out. All right, these ones.
[31:46] - Yeah, you see, we've got two terminals running them. One of them says node.
[31:50] If we click on that, you should see that it's compiling the website.
[31:57] So it's building it so that we can test it live. This is all done automatically.
[32:02] - That's cool. - Yeah, so it's doing that for us.
[32:05] And in the end where it says task and the other terminal that says task two,
[32:10] that is our, that's our terminal that I set up for us so that we can, you know, do terminal things if needed.
[32:18] - I dig it, I dig it, okay. - So let's go back to that Gitpod task one real quick.
[32:26] The terminal there, you know, the one that we opened before. - I think it, Gitpod just closed it, so.
[32:38] - Oh, no, no, it didn't. If you go back to Gitpod real quick.
[32:42] - Yeah. - You see it at the bottom right.
[32:45] You see, we had those two terminals, right? I just wanted to go back to the, yeah, that one.
[32:52] - Oh, okay, I thought you meant going back to the issue. - No, no, my bad.
[32:58] Scroll up just a touch. - Okay.
[33:03] This one, this one? - Yep.
[33:06] - There we go. - There, you can now view DA landing in the browser
[33:10] where it says localhost 8000. Go ahead and hover your mouse over that and press command,
[33:16] like hold down command and click on it. So that's gonna open up a fake local host
[33:27] that's running in Gitpod in your browser. - I see, okay.
[33:32] - So this is the website as it is right now in development mode, as if you were running it,
[33:38] you know, locally on your machine, but instead you're running out on Gitpod.
[33:40] So why are we using Gitpod? What I like about it is that it lets me and Taylor,
[33:45] like share this link and work collaboratively. - This is really fun.
[33:52] We're gonna do some real hacker stuff. So I think that you need to turn on the sharing
[33:58] for the Gitpod instance, right, Ramon? - Yes, that is if we want to hop in.
[34:04] - Yeah, is that a good, I probably need to be able to hop in
[34:10] to just copy and paste some content later on here. - Sounds good.
[34:14] In that case, Jen, at the bottom of the window, you'll see where it says like Gitpod saga,
[34:20] and then there's some symbols and it says share. - Share.
[34:26] - Yeah, so if you copy that URL to the clipboard and maybe paste it in the private chat here,
[34:31] we can hop in and collaborate with you a la Google Docs. - So Finn asked a good question.
[34:42] Is it difficult to set up Gitpod? - That's an excellent question.
[34:47] - This was super easy. Ramon did a little bit of magic and it was there.
[34:53] - It's honestly not all that much magic. Like their docs are super straightforward to set up.
[34:58] You'll see that there is a, and that's a file you almost opened, Jen.
[35:01] There's a file called .gitpod.yaml here in our Explorer. - Yeah.
[35:09] - I think you see it there. Yeah.
[35:11] And what, I mean, you can see there what it is. We've got two tasks, like the two terminals that you saw.
[35:21] One is, one does Yarn install and then Yarn dev to start up, you know, Yarn install.
[35:27] Have you worked with Yarn yet, Jen? - Yeah, technically, yes.
[35:33] - Okay. So you know that it's kind of like an alternative to,
[35:37] well, yeah, an alternative workflow to NPM. - Yeah, and in Python, it's pip or pipX.
[35:46] - And in Ruby, it's gem. - See? - Which is cute.
[35:50] - All the learning. - I think in Elixir, it's hex, though I could be wrong.
[35:55] - Yeah, it is hex. - Anyways. Oh, nice.
[35:59] And in Rust, it's cargo. Okay, I'm done.
[36:00] So yeah, what we can do is define here how Gitpod should set up.
[36:06] - And then I think that all it took was going to Gitpod and saying, hey, can you, you know, giving it access
[36:14] through like one of the GitHub apps or something like that, right?
[36:17] So basically, you let Gitpod, you know, you connect it to your repository.
[36:22] That's just a few clicks of a button. And then we added that button to our README,
[36:29] which I think is just linking a specific link to Gitpod so that when you go click that button,
[36:35] it opens up the Gitpod and it knows what repository you're part of.
[36:38] It grabs the data and the files from that repository to set it up in the local code editor.
[36:44] And it runs the commands that you've given it in that Gitpod.yaml file.
[36:51] - Okay, that kind of made sense, but I'm going to go with it.
[37:00] - Awesome. Let's, in that case, I don't know, Taylor,
[37:07] how shall we proceed? I've been talking for a while.
[37:10] I don't want to dominate too much. - I think we can start maybe by diving
[37:17] into the issue. And what we like to do, Jen,
[37:20] is we like to create the branch that we're going to be working on,
[37:26] and then go ahead and open an in-progress pull request just right away.
[37:31] And that's designed to make sure that people, like, you know, aren't just going off
[37:35] and working on stuff by themselves, but, you know, people can show their work
[37:39] as they're working towards an issue, and we can see it and, you know,
[37:42] get other folks involved, right? So if you go open a new tab in your browser
[37:48] and go back to the github.com/distributeaid/distributeaid.org. Oh, wow, that was magic right there.
[37:58] - I bookmarked it. - Cool, very cool.
[38:02] And so we'll go to issues, and I think it was 523. It should be the first one right there.
[38:09] - Yeah, we can see the issue number is 523. - Mm-hmm, exactly.
[38:17] So what we'll want to do is on the Gitpod, we'll want to check out, like, create a new branch in Git
[38:26] related to this issue, and check it out, and then push it right away.
[38:32] So on the bottom right, you can go to Gitpod task two. That's our, a little bit above right there, perfect.
[38:42] Yep, and so if you click on that, that's our terminal. So here, have you used Git on the command line before?
[38:48] Yeah, you're doing, okay, perfect. So we can create a new branch here off of saga.
[38:55] Saga is the name of our main branch. It's kind of that Viking storytelling sort of word.
[39:02] So that's what we call our main branch. - Do you remind me?
[39:04] Because, like, I've done it, but not enough to, like, remember all the steps.
[39:09] - 100%, so we're going to run git checkout -b. That'll tell it to do a new branch,
[39:17] and then we're going to want to name the branch after that. So let's add another space.
[39:22] We don't really have solid naming conventions, but what Ramon and I like to do
[39:28] is indicate that this is a feature branch. So we'll type in feat, F-E-A-T,
[39:34] and then do a slash, and then put the issue number there. So that would be 523.
[39:40] Yeah, dash, a slash, it's all the same. And then add another dash or slash,
[39:47] and kind of describe what we're doing. And we're essentially creating, like,
[39:55] ways to get generic content on a page. This is always the hardest part for me, Ramon.
[40:02] What should we- - I actually have an idea.
[40:05] How about page-template? - Yeah, there we go.
[40:09] - So that's going to be our new branch. - Mm-hmm, and so what that'll do
[40:17] is it'll create a new branch, and it'll check it out at the same time.
[40:20] You'll now be in that branch. - We're creating the template, right?
[40:25] - Yes. - Okay, so I added creation.
[40:28] - Love it. - Yep.
[40:31] - All right, and then enter, I'm guessing? - Yep.
[40:35] - You know, on that one, yay! Perfect, there you go.
[40:40] So now, go for it, Ramon. - Sorry, I was just going to say,
[40:44] so even though we've checked out this branch, it's only locally in our Gitpod.
[40:51] It's not pushed to GitHub yet. - Okay. - Back to you, Taylor.
[40:56] - Yep, so the next step is to push it to GitHub. And this is especially true on Gitpod.
[41:02] You don't want to leave work that you've committed, even, that you haven't pushed back up on Gitpod,
[41:08] because this instance will go away. It's running on some virtual machine in the cloud,
[41:13] and, you know, 30 minutes after we're done with it, that virtual machine's gonna get deleted
[41:18] to make space for someone else's Gitpod. So if you run, I never forget the right command
[41:24] to push a new branch, but the nice thing is we don't have to.
[41:27] If you just run git push, it'll tell us what that command is
[41:31] when you have a new branch. There we go.
[41:35] So it's like, there's no upstream, there's nothing on GitHub for this branch.
[41:39] We basically need to say, hey, push it to this location. That's what it's telling us to do.
[41:45] So you can type out or copy and paste that git push set upstream origin, and then the name of the branch.
[41:53] - And, you know, usually I'll be the first one to say like, oh, you know, it's a good idea to type something out
[42:05] instead of copy pasting it. But something like this, totally fine to copy paste.
[42:12] Okay, so we've got an error. Is not accessible with the current tech
[42:19] and please grant the necessary permissions. Now, Taylor, you said that you invited Jen
[42:24] to be a contributor. - Oh, that's true. Jen, I invited you, you need to accept the invite.
[42:29] There we go. - Ooh. - So either your-- - Your emails,
[42:34] you'll get an invite. - Yeah, or maybe on GitHub if there's a notification or something like that.
[42:39] - Yeah. - I had a notification earlier. Maybe.
[42:44] - Checking, I invited the right Jen. - It is teach-jen-tech, right?
[42:51] - Yeah. - Yeah. - Oh, okay, I think that maybe I invited the wrong Jen.
[42:58] My first name, last name. - Yeah, yeah.
[43:02] - That's not the wrong Jen, that's just a Jen that I don't have access to.
[43:06] - Oh, okay. - And then there's Jen with multiple Ns in my last name
[43:10] and I don't know how I created that one, but I need to merge them.
[43:15] - Let me read this real quick. - I do wonder if it is possible to merge GitHub accounts.
[43:22] - It would be nice. - Yeah. - But-- - I did many,
[43:31] like, I have two GitHub accounts myself. I created one as a gag many years ago to,
[43:37] it was called Evil Ramon and it was for a presentation I used to do
[43:43] on teaching Git to beginners. And I would sort of go, like, this is when I had short hair
[43:48] and I would go off stage and I would put on a wig and I would come out and sort of mess up the Git history
[43:55] just to, like, it was a way to demonstrate how Git works. - Yeah, yeah, it totally makes sense.
[44:00] - It was cool. I think I still have that wig.
[44:03] It's like a big roadie wig. Anyway-- - Kai doesn't believe
[44:07] that you have an evil side. - Kai should know better by now that I do have one.
[44:14] - I would say, don't we all technically, we just may not know about it.
[44:22] Be in tune with it. There we go.
[44:25] - So you're invited now, Jen. And I totally agree, we all have an evil side.
[44:31] I like using my powers of evil to bully companies into giving me tons and tons of stuff for free.
[44:38] It's like the, you know, we do nice things all day and I'm like, no, actually you can afford
[44:42] to give us your misprint product, right? Instead of throwing it away.
[44:47] - Two wrongs make a right. - And I also do agree that I like to use
[44:51] the power of email as well. - No. - No.
[44:54] - Because I don't like using email very often. So it's, you know, I wait it out.
[45:01] Okay, let me see if I have any emails. - So now you invited Teach Gen Tech, right?
[45:12] - Teach Gen Tech, yeah. - Perfect, that should get you an email notification
[45:19] saying like, you know, you're invited to join on this organization.
[45:25] So you'll accept it and then they'll ask you for a step for accepting it.
[45:29] And then you'll be able to push that branch. - Once I set up my two-factor authentication.
[45:36] - Very important. - Oh boy. - What kind of, no, I'm not gonna ask that live on stream.
[45:41] Sorry. - What?
[45:44] - What is that five-digit code they just sent you? - No, I was gonna ask like, what method do you have?
[45:49] 'Cause I'm just nosy and curious, but like, really, we shouldn't be asking that.
[45:53] - I actually asked companies to send me a letter in the mail to authenticate.
[45:59] - Okay, I saved it. - Are you in? Okay. - Done.
[46:08] Okay, I believe I can now go back here. - I guess a very realistic look
[46:17] at contributing to open source. Everyone thinks you're like, you know,
[46:20] some open source rockstar or something. Like, no, it's mostly just figuring out
[46:24] how GitHub's UI changes, you know, broke your flow or something.
[46:28] - Absolutely. - I'm trying to see if I can just click up.
[46:33] - That should be working now. Let me double check that it's coming through on my end.
[46:42] - I'll do the same. - It says you're pending, Jen.
[46:46] So I think you set up your two-factor offer. Do you accept the invitation to distribute aid after that?
[46:52] - Well, it says join distribute aid, and then to join, I will do it again.
[47:00] I already had two-factor on it, whatever. Okay. - Maybe it's asking you to.
[47:05] - Oh, now it's working. Now it looks like you're on there.
[47:08] So I think we're- - You are absolutely right. It was like, no, you have to go back and do it.
[47:13] It didn't tell me that, but. - No. - Whatever.
[47:18] No. I'll give it a second.
[47:28] - Wait, wait, the error looked different this time. Could you try again, Jen, please?
[47:31] - Yes. - Okay.
[47:35] An operation requires additional permissions. Let's go on open access control.
[47:42] - Good spot, Ramon. - 'Cause it could be that, now that you have access to it,
[47:47] you see where it says- - Yeah. - Git providers, if you go there and click on,
[47:52] no, we're not doing GitLab. We're doing GitHub. - But the GitHub
[47:55] on the dot, dot, dot there. - Mm-hmm, edit permissions.
[47:59] And now we can go public repo. - And it went public repo. So it can write code to public repositories.
[48:06] Nice. - Then GitHub's gonna be like,
[48:09] are you sure you wanna do this? And you would be like, yes, I do.
[48:12] - Sweet. - So now we go back and try again.
[48:19] - Hey. - Wonderful. - There we go.
[48:25] There we go. Let's go take a look at your new branch on GitHub
[48:29] and set up a work in progress pull request. Ramon, did you have anything?
[48:32] I didn't mean to cut you off there. - No, no, you're good.
[48:35] I was gonna suggest the same. - Awesome.
[48:39] - There we go. - I didn't know about this. - Feature 523 page template creation.
[48:43] - This is cool. - Yeah, all I did was over here,
[48:51] you can see your six branches. - Yeah, that's super handy.
[48:55] - And then this is my branch. And you said you wanted me to create a new pull request.
[49:03] - Yep, just right off the bat right there. And what we'll do is we'll mark it
[49:08] as a work in progress pull request. And so that's really cool
[49:12] 'cause it means you're sharing your code, people can see what you're working on, right?
[49:17] But they know that it's work in progress, you're gonna be adding to it.
[49:22] So I think it's set up. Oh, do we need to have some sort of diff before we do this?
[49:26] - We'll need a bit of a diff, yeah. Why don't we start with the thing straightforward
[49:30] and add Jen to the contributors list? - Perfect, perfect.
[49:34] That's an easy starting point. So go ahead, Taylor.
[49:40] - Yeah, I was wrong. So we can't, like, since we just branched off
[49:43] our main branch and there's no changes yet, GitHub's like, ah, you can't make a,
[49:48] kind of essentially an empty or a null pull request here. So if you could go back to the git pod gen,
[49:55] we're gonna just have a really quick first commit here. If you scroll down to contributors.md,
[50:03] this is something we ask everyone who contributes to distribute aid to add their name to.
[50:10] So this is our way of making sure that, you know, people are abiding by our code of conduct
[50:18] and, you know, just kind of generally respect the space. It also has a copyright transfer provision
[50:25] because we want the org to be able to handle any licensing issues or anything like that.
[50:29] So all the code's open source. It's actually a really good open source license
[50:34] called the AGPL, which really prevents companies from, like, taking our lovely nonprofit open source code
[50:41] and using it, like, privately without sharing back. It kind of requires everyone to share their code back here.
[50:51] And we're good stewards of it. But by adding your name here,
[50:55] you agree to our code of conduct and you're happy to assign copyright
[51:01] to any code you contribute to distribute aid organization. - So do I have to save it here?
[51:15] Sorry, like, I understood what you were saying, but then I was like, wait, do I save this?
[51:21] Like, I have to save VS code. And that was a yes, still save it?
[51:26] - Yeah, I think you just save the file like normal. - I do wanna point out, if I may, Jen,
[51:34] you're missing a space before you have the J in your name. - Oh, thank you.
[51:38] - And then we, even though you've saved this, you still need to make a commit.
[51:43] - Okay, and- - Do we wanna do this in the terminal
[51:48] or do we wanna use VS code's built-in Git stuff? What do you feel more comfortable in?
[51:55] - I feel like I should do it in terminal to get used to it. - Yeah, there we go. - Let's do it.
[51:59] - I love it. - So if I do the same thing I did earlier
[52:03] without having to remember what it is, it's if you git push.
[52:07] - Well, not quite, we still need to create that commit. - Oh, okay.
[52:11] Is it git commit? - So the commit is like, that's your save point
[52:14] in a video game or something like that, right? So it's like, this is that checkpoint right there.
[52:20] Yeah, I think it's git space commit space, and we don't really do super long commit messages,
[52:30] but if you do a dash M and then run, yep, go for it. - Don't forget the add.
[52:37] - Oh, yeah, let's see. - Git commit add or git add commit?
[52:41] - There's no commit yet. So delete the commit.
[52:45] - We should really start with a git status, right? - Git status is a good starting point, yeah.
[52:55] - Git status. - So those are the files that we've changed.
[53:01] Now we're going to be adding the file contributors.md to be committed.
[53:07] - Yep. - So git add space and then type capital C
[53:14] and then tab and that'll auto-complete it for you. Yeah.
[53:20] - And then do I have to do a dash M or anything for this one or just enter?
[53:24] - Just enter, yeah. - Okay, and now I can go to git contribute, wait,
[53:32] git commit. - Git commit, yep.
[53:36] Dash M and then you'll want to have an open quote and let's take a minute to think about
[53:44] our commit message here. So for the commit messages,
[53:50] there's this thing called conventional commits, which is pretty cool.
[53:54] - I'll get a link. - Yep, there we go.
[53:56] Ramon will get the link. The idea is that we don't need the 80 character title
[54:03] and multiple paragraphs explaining what's going on. We do want to leave a nice trail of red coms
[54:09] for people to follow. So conventional commits is a style
[54:13] of making these commit messages, which is consistent, regardless of who's contributing.
[54:19] So we're going to start off by, what would, this is not quite a feature, Ramon.
[54:25] Would this be appropriate for like the chore label? - Documentation, docs.
[54:30] - Yeah, there we go. So if you type docs and then a colon
[54:35] and then say what you did and that's all. Yep, so.
[54:39] Perfect, that's great. And then let's end that quote there.
[54:56] And that's it. So git commit and then -m is the shortcut
[55:00] to just write a commit message directly in the command line there.
[55:04] If you, yep, nice. There we go. - Yay.
[55:09] - What happened there is we have some kind of commit hooks. So we're actually running some automated,
[55:17] what's it called? Like code, it's not code linting,
[55:21] but it like does the code formatting and some checks and stuff like that.
[55:24] And so, yeah, it just kind of cleans everything up, each commit, which means you don't have to worry so much
[55:31] if like things aren't quite aligned when you're typing the code.
[55:35] You know, if you prefer to like write your functions all in one line or spread them out on 20 different lines
[55:41] or whatever, it kind of has, so we have this standard code formatter,
[55:45] which runs at the end. So you can just focus on getting that code done
[55:49] and then it'll, when it goes and you commit it, it'll kind of like put it in a standard style.
[55:55] - So Jen, I noticed you're, I think you're, I think you went back to GitHub.
[56:02] We still need to push our commits. - Yeah. - I know.
[56:07] - I just really want to do a new, so is it git push now? - Yeah. - Git push, yeah.
[56:13] - No. There we go.
[56:18] - There it is. - There we go, love it. Your first commit to DA, Jen, welcome board.
[56:25] - Yay, I still don't fully, like I'm starting to understand this,
[56:29] but I don't fully understand this, but now I can actually do a new pull request.
[56:34] - Yep. - That's right. - Exactly.
[56:35] - Do y'all know, oh, one commit ahead, one commit behind Saga.
[56:43] Interesting. Let's click on new pull request, yeah.
[56:50] - Hey, it added you in there, and then create pull request, right?
[57:00] - Not quite, we do want to, sorry, go ahead, Taylor. - No, go for it, go for it.
[57:04] - Well, the title of our pull request currently says, agree to be a contributor,
[57:11] which is technically correct so far, but for the overarching, I'm sorry,
[57:18] I'm going to go with overarching, actually. The overarching goal of this pull request
[57:23] is to create that page template. So I would go with,
[57:29] instead of docs agree to be a contributor, let's call this pull request, create page template.
[57:35] You can remove the docs part too. - Yep.
[57:40] - Perfect, oh, yes. Where do we make it into a draft?
[57:52] - I can't remember if we're able to do that. Maybe, yeah, the arrow there, create draft pull request.
[58:00] There we go. - Thank you, Jen. - And then would it be smart
[58:04] to put the issue information here? - Yep, I think that's a great call.
[58:10] You know, if you want to say like for links too, then I think you can do the first line 523 or whatever,
[58:16] it kind of-- - Do you know the magic? - It was where, yeah.
[58:23] - I love this feature of GitHub, that it automatically makes a link when you publish it.
[58:29] - And cool. - Yeah, I think that's good.
[58:35] - So we're going to do a draft? - Mm-hmm. - Yep, exactly.
[58:40] - So now at this point, what we've done, your code environment's set up,
[58:44] you say, "Hey, I want to work on this issue, get assigned." Cool, like you're in charge.
[58:50] And now you have this space, you know, like showing your progress as you make commits
[58:55] and contribute to this pull request. And that's really cool because it lets you
[59:00] like ask for help on the way. You know, "Hey, can I get a second pair of eyes?"
[59:04] Right, you don't have to wait until everything's done and then do the big pull request review
[59:09] and then get it merged. You're like, "Well, I'm kind of stuck on this point.
[59:12] "Let me push what I have up "and it'll be visible on GitHub
[59:15] "and tag in Taylor, tag in Ramon," right? Yeah, I don't think at this point
[59:22] we need to add any labels or, you know, the reviewers is just kind of like with, you know,
[59:29] saying who wants to work on an issue, Ramon and I and other folks at DA are like,
[59:33] "Oh, who wants to like review this pull request?" So we'll kind of jump in there.
[59:37] You know, when we have time, one of us will pick it up. Yeah, I don't think there's too much more
[59:46] on the setup side here. Maybe we should take a look at the code C map real quick
[59:52] that's in the issue and that'll kind of show us where we're going to be working in our code base.
[59:58] So if you go back to the issue, Ramon and I are big fans of code C.
[60:06] Also, full disclosure, they do sponsor our stream and our work at DA, love them to death,
[60:12] but we use their tools because they're useful. And so what I've done here is added a link
[60:18] kind of below the intro bit. And so code C has this great code base mapping software
[60:26] and I've highlighted some of the different files or folders or just like the right parts
[60:32] of the code base to look in. That way, you know, I mean, a landing site like this,
[60:38] we have lots of different things going on. You don't need to know 90% of the code base
[60:43] to contribute to a lot of these open source projects, right? So helping folks jump in and find out
[60:49] what's relevant to the issue they're working on is super important, and this is how we do that.
[60:54] And then I set up a little tour to kind of like walk us through,
[60:57] like let's take a look at some of these files and then some of those files.
[61:01] And, you know, as we refactor and kind of refine the pull requests, how it might take shape.
[61:06] - The name of the game here is onboarding, sorry. - I was just gonna say like this,
[61:15] your words make sense, what they mean, not there yet. But I think that's like the cool part
[61:22] that I've really learned, especially since like Ramon was first on the show
[61:26] is it's like, it may not make sense right now, but doing it like a few times, maybe in a week or two,
[61:32] nine times out of 10, it'll make sense. - You're gonna be coming back.
[61:35] - That's the fun part about learning, right? Sorry, go for it Ramon.
[61:39] - No, no, you're totally right. No, what I was gonna say was like, you know,
[61:41] a lot of these concepts you're gonna keep coming back to you're like, oh yeah, I've done a commit
[61:45] before I kind of went like this, right? - Yeah.
[61:48] - That's the learning. - Yeah. - Exactly, exactly.
[61:54] And I totally spaced doing my readme, damn it. At least these are recorded
[61:59] so I can go back and watch it. To create my readme for myself.
[62:04] Okay, so what do I do from here? - Yeah, so this is a CodeSeaMap with a tour
[62:14] and I've hidden a lot of like the, you know, settings and configuration files and folders
[62:19] that you don't really need to worry about. So this is, you know, basically the files and folders
[62:26] that are relevant to what we're working on. It's like what you see in that sidebar
[62:30] on the VS Code Editor or in kind of the GitHub file system view,
[62:34] but it's laid out and you can see this map and how those files relate to each other.
[62:40] We have a little tour. So if you wanna click the number one bit right there, yep.
[62:48] So that was kind of the first thing we're planning on doing today.
[62:52] You might need to drag, maybe you need to use the hand function.
[62:57] There we go. - There we go. - Nice, yep.
[63:00] So number one, review key docs and add gen to the contributors MD.
[63:06] Already went through it. - Yay. - Yeah, yay.
[63:11] Next up, what we're working on now, create a generic page with hard-coded content,
[63:19] style it, possibly wrap it in a layout, right? So we just wanna say, cool, like what types of content
[63:25] are we gonna see on an about us page or a guide page or some of these kind of one-off pages.
[63:32] I have some of that ready. So we can go ahead and make a new page in Gatsby, in React,
[63:38] do some tail and styling, kind of figure out how this works.
[63:42] And then we can kind of walk it backwards and make it more of a template as we refactor it.
[63:49] But I really like this style, especially for folks who are learning how to code
[63:54] because it makes it real. You don't have to do all of this abstract stuff
[63:58] to get to the real part at the end. Start with the real part,
[64:01] put HTML and content on the page and then refine it and refactor it
[64:07] and make it more generic and abstract as you go. - I am like noticing that it took us like an hour
[64:17] to get all that set up because it is like asking so many questions
[64:20] that we don't always know that we'll ask. Like it's, yeah, like, 'cause I just looked up
[64:27] and I was like, it's been an hour already. What happened with time?
[64:31] Where'd it go? - Time flew.
[64:34] - Yeah, happens when you're having fun. - I was, I wanna say like something funny
[64:40] about like time codes or something like that, but I'm like, it's not coming to me.
[64:45] I just really wanted it to be punny. It didn't work, it's okay.
[64:50] Moving on, I need to create a generic page with hard-coded content, style it and wrap it,
[64:57] possibly wrap it with a layout. - No. - Okay.
[65:01] Then I'm guessing I don't need this Git pod, I need this Git pod.
[65:07] - There we go. - And I don't know where I'm going from here.
[65:14] - That's okay, that's what the CodeScene app was for. - Okay, so let me zoom in on this.
[65:23] - All right, so. - Shall we end the tour real quick
[65:26] so that we can see the full files? So you see, Jen, next to, near the top,
[65:31] there's an End Tour button. - Oh, and then I can click it under Pages.
[65:39] - Yeah. - Well, before Pages, there's SRC.
[65:42] - Oh. - Because Pages is inside SRC. - Yeah.
[65:48] - Okay, so all of these would be, I'm just wanting to compare them side by side really quick,
[65:56] because I think that's also something that can be hard with these visualizations
[66:01] if I'm not looking at them in the same format. - Mm-hmm. - So, go away.
[66:06] Thank you. And then we'll do these, and these.
[66:12] All right, so like, Code, can you move Legend? Hi, Legend, can you?
[66:17] No, no, you won't move for me, thanks. No, it's for Code, see?
[66:21] - Yeah. - Like, even if they can just, like,
[66:26] minimize it, like this one minimized, that would be nice. Okay, so the, we have, of course, the, like, full file
[66:37] with all, like, the files in it, but the README's here. Code of Conduct is here.
[66:47] So this is showing that all of those are outside, just in the primary folder.
[66:52] Cool. - Exactly. - So-- - Usually called the root folder.
[66:56] - Root folder, yeah. Okay, and then, so this one, I like this,
[67:01] because it's showing that it's in SRC, and then eventually we'll go into Pages,
[67:07] which is in our SRC layouts. - Mm-hmm. - So, sweet.
[67:12] We're here, we're gonna expand it here again. And, oh, that's also very difficult to see.
[67:21] Just kidding, I don't know, I'm not gonna do this. Maybe that, I don't know. - Oh, yeah.
[67:33] - It let me change things, and I didn't want to change. No, go, I just.
[67:37] There we go, okay. - There we go. (laughs)
[67:43] - Nice. So, it tells me what's in this folder.
[67:49] I feel like I'm not seeing what I would edit in this folder. - No, but I think that's perfect.
[67:57] We want to add a new page to this folder, essentially, right, just give ourselves some working space,
[68:02] you know, to start off with something. So that's what I was trying to show you,
[68:05] is here's the SRC folder, and then here's Pages. That's a relevant thing, let's go look at that together.
[68:13] But just so you're not looking through all the other dozen folders, like Gatsby,
[68:17] or Content, or things like that, yeah. - Okay.
[68:22] - So. - So, new document? - Yeah, yeah, if you open the Pages folder there,
[68:33] and let's add a new file to it, and just get a hello world going on our page.
[68:41] - Okay. What are we naming?
[68:45] - Why don't we call this? - Page?
[68:50] - Yeah, page, page. We could call it tech, let's do tech at distribute eight.
[68:58] So like, you know, our-tech or something dot TSX. - TSX, yeah.
[69:11] It's like JSX, which is the kind of React naming thing, but with TypeScript.
[69:18] - Ooh, okay. - Wonderful. - So we have, we've made it.
[69:24] We- - Made it. - We're here.
[69:27] Now I don't know what I'm doing. - That's perfect.
[69:30] I think a good starting place might be to do a little bit of copy-paste-modify,
[69:36] or at least look at, you know, some of these other one-off pages,
[69:42] and that'll show us the sort of like, the imports we might need, you know,
[69:46] start with what's already there, maybe. - The only reason why I'm going back here
[69:54] is thinking like, it might be easier to visualize what page to copy and modify.
[70:01] - I like that. - Because in my mind, I don't think all the template pages
[70:08] would necessarily need the world. - Exactly. - For distribution.
[70:13] - Even though it looks so good. - Awesome.
[70:16] That's what Robon and I were putting live on our last stream, so.
[70:21] - Well, I do have a request for this of, can there be arrows?
[70:25] Like where, it's because like this one right here just looks solid, so I don't know like that,
[70:36] like if they're moving or whatnot, like that kind of thing.
[70:40] - I'll tell you what, Jen, if you add an issue to the distributed signing site,
[70:45] then I will put arrows on it if I can, or something like that.
[70:50] - Okay. Make sure I'm in the right folder.
[70:57] So. - Is it cool if y'all, I'm gonna go refill my water real quick.
[71:01] - Ramon. - Go for it, go for it, I'll take over. - Can you work
[71:03] the channel on the issue? Perfect. - Yeah.
[71:05] So let's go to issues, and then you can click on new issue.
[71:09] So a couple of things. First off, we need a title.
[71:17] What do you think? - Landing page globe.
[71:22] - That's not, like that is the area that has an issue, but it's not the issue itself.
[71:31] Like what is the issue that we wanna solve? I would say, for example,
[71:36] make globe arrow, make globe, what are they called?
[71:41] Arcs clearer. - Could we do add arrows to arcs on globe?
[71:53] - Absolutely. - Okay.
[71:55] - Okay. - But yeah, it's always,
[72:04] like whenever I'm writing an issue, I always ask myself, like what is it that needs to be done?
[72:10] Are you gonna take a screenshot? - I was.
[72:13] - Fantastic. Absolutely do.
[72:15] Ooh, what is this? - It is Snagit.
[72:24] - I don't know if you'll be able to see my Snagit screen. There we go.
[72:28] - Very fancy. - And then I can do like these things.
[72:34] - Nice. - I don't know if it will do it,
[72:41] but a lot of times I can copy and paste it. So I'm curious.
[72:46] Oh, it's uploading. No, it didn't work.
[72:49] - No, it did. - It did?
[72:51] - So yeah, if you want a preview, you're gonna see it. - Ha ha.
[72:55] - However, let's go back to write. We have an issue.
[73:00] - And I gotta tell him what it is. - Well, no, we have an issue in our image.
[73:04] You see, we've got the bang, the exclamation mark, and then in square brackets, we've got the alt text.
[73:14] You know what the alt text is? - Yes, to make it accessible for everyone.
[73:22] - Yeah, so it's saying image isn't very accessible. So what are we describing here?
[73:31] - Globe with arcs showing distribute aid. (indistinct)
[73:51] - Shipments. - Thank you.
[73:57] - Could it be, it should be arches? Yeah, but arches sounds like a church.
[74:09] I don't know, I'm not very knowledgeable. - It clicked it and went to its own thing.
[74:17] But is there a way? - What is it you wanna do?
[74:21] - Just to see if the, since it opened up over here to see if it would show the alt text.
[74:28] - Yeah, if you go back to GitHub, then go on preview and then right click on the image
[74:36] and then go on inspect. So the Grumpy MB is saying arrows,
[74:42] but like they're not arrows yet. That's the problem.
[74:45] - We're adding the arrows. - And a good call.
[74:48] Yes, marketers love Snagit. It's true, but I actually learned it
[74:52] from the CTO of some company because he was trying to teach me about SDKs
[74:58] way back in the day because I was in charge of like making this website work with Zoom.
[75:03] And he is the one that taught me about Snagit. - Hey everybody.
[75:09] - What up? - What up?
[75:11] I was able to still hear you and Ramon. How do you hear the word arches
[75:16] and think church instead of McDonald's? - Why?
[75:21] - It's the golden arches. Is that not a thing?
[75:24] That's a thing, right Jen? - So I honestly did not realize they were golden arches.
[75:29] So the M of McDonald's are two golden arches. Other than the only reason that I know
[75:35] they are golden arches instead of just an M is in Sedona, Arizona,
[75:42] it is the only arches that are teal and not yellow because they needed to match everything around.
[75:51] So it's kind of like FedEx. Have you ever seen between the E and the X
[75:58] that there's the arrow? - I have never heard of the golden arches.
[76:04] - Yeah. - It's not a thing in Europe, I guess.
[76:06] You gotta come to the States sometime. - It's not a thing in Chile either.
[76:11] - Yeah, like I don't know if it's necessarily a thing because when I was in Idaho or Colorado or Indiana.
[76:20] - The Grumpy MBA definitely has and they're in Austria. So maybe I just missed it.
[76:28] - I don't think it's as commonly talked about anymore. - Yeah, probably not.
[76:33] - 'Cause I didn't learn it until I was like 28. So I don't know.
[76:42] But fun fact, is there another fun fact? - You can buy beer at McDonald's in Serbia.
[76:49] It was very surprising to see it on the menu. Really?
[76:52] Is that just European McDonald's? It definitely doesn't happen in U.S. McDonald's.
[76:56] - Does it happen in Germany? Because I remember going to one of the clubs there
[77:00] and then very drunkenly eating McNuggets. But I don't remember if there was beer there too.
[77:10] It was in Munich. - Sounds pretty close to me.
[77:14] - Sounds like a fun way to use it. - Yeah.
[77:17] - It was, it was, it was. But not good idea for anybody that wants to go party
[77:24] or do anything, eat more than sushi before you go drink a lot.
[77:29] - Some pasta, some pizza, you know. But I'm going to create this issue.
[77:39] This issue and I are going to get along. - Yeah, let's go ahead and close the DevTools.
[77:44] - Yay. Kai, one day we will all meet up and get some sushi.
[77:54] See if I can talk some sushi. I think that is, it's so weird having like internet friends
[78:00] because it's like, oh, I'm getting to know them really well. I've never met them in person.
[78:06] - Wait until you play the game of when you meet them in person and you realize
[78:11] they're not the height you pictured in your head. - This is 100% true.
[78:16] Also, I'm going to start playing Dungeons and Dragons on Friday nights.
[78:20] - Fun. - And I'm just like,
[78:23] it's so fun to be able to nerd out more with the internet world.
[78:28] I don't know why I'm like so behind the times on this, but we are going to say,
[78:35] please add arrows to point to where the shipment is starting and ending.
[78:55] That work? - I love it. Yeah, it's great.
[79:00] And I got to say to the audience, like there's so many ways you can contribute to open source
[79:05] that don't involve writing code. Like one of the biggest challenges for everyone and I,
[79:10] you know, maintaining this landing site project for distributed aid is just making sure
[79:14] that there are fresh issues for folks to pick up and work on.
[79:18] So things like, you know, if you see it, say it, right? If there's something we can improve on,
[79:23] submitting an issue like this is a great way to make a very real contribution and get that ball rolling
[79:28] towards getting the issue resolved. You know, reviewing code, right?
[79:32] You don't have to write the code, but pick up a PR, do a review, give people some feedback,
[79:37] learn together with them, you know? And of course I got to give a shout out
[79:41] to my admin and ops team who do a whole lot of, you know, data formatting and kind of getting
[79:49] the information that we need to work on pretty visualizations like that globe.
[79:54] You know, so I think when people think of open source, they think of GitHub, they think of writing code
[79:58] and, you know, really working with Ramon, we've had a lot of conversations
[80:02] about like the million other things you can do to contribute to open source projects,
[80:08] you know, that don't require opening a code editor. - Would, thank you for that.
[80:17] And would you put in like where it is in the folders normally or you just let whoever
[80:25] is gonna work on the issue, figure that out? - Um, I think that that doesn't hurt,
[80:32] but I also don't think it's a requirement. So that's something that Ramon and I do,
[80:35] like our next step in this process would be to like review the issue you submitted
[80:40] and go add in supporting stuff like those code C maps to make it easier for people to pick up
[80:46] and get started with. So I'd say like, get it in there, you know,
[80:50] and we can kind of collaboratively build out the issue together.
[80:54] Yeah. - Okay.
[80:57] - Enhancement. - Yep.
[81:03] - And is it a good first issue? - I'm gonna say probably not.
[81:07] Yeah, because it gets in the 3D kind of visualization, but we can say help want it though.
[81:12] So it can not necessarily be a good first issue, but anyone could pick it up if you feel like a challenge
[81:18] or if you feel confident with your 3D kind of, you know, library sort of skills.
[81:25] And I'm guessing the only reason I can see these is because I was put as a dev for it,
[81:32] not like somebody that just came in probably would it. - Exactly, yeah.
[81:39] I think that's usually if someone just submits an issue, then Ramon and I will go label it and then stuff like that.
[81:45] - Sweet, yay. I created issue 527.
[81:50] Too bad it wasn't 528, it would be my birthday. I mean, you can make another issue right now.
[81:56] - But it would be in like US way, not everywhere else. It's still so confusing talking to the rest of the world
[82:03] with dates. All right, so just as a pause really quick
[82:10] before we move forward, because I feel like we did that. And are we stopping at half past or 45 past?
[82:18] Because we haven't, we started a lot, but yet didn't start a lot.
[82:27] - I mean, this is, first off, this is an ongoing thing. Right, we can go as far as needed
[82:32] and then we can keep that going from there. Second of all, we did start a lot,
[82:39] but we also did finish quite a lot. Like we created a new branch.
[82:43] We made a new, we added you as a contributor. We did a lot.
[82:48] - Yeah. - Lastly, Jen, you're the boss.
[82:52] This is your stream. We're happy to hang out until you tell us
[82:55] it's time to go home. - I mean, that is fair.
[82:59] I feel like at this point, it's, I want to, if we break this up more, I'm gonna get kind of confused
[83:07] without being able to finish this portion of it. And I ask a lot of in between questions
[83:16] that help with the overall like concept, but doesn't help get the actual task at hand done,
[83:25] but will make it faster in the future. So on that note, I vote that we pause here.
[83:32] I'm gonna actually not save this file just because I would love to start up
[83:38] with having to start this file. - Yep.
[83:42] No, it seems like a really great stopping point. Like, cool, we're all set up, we're ready to go.
[83:47] You're a dev, you've kind of figured your way out around the code base, you know what Gitpod is now,
[83:54] and we can jump into this. (laughing)
[83:59] - That was so scary. - Yeah.
[84:03] I think we're doing like a Flexbox layout there, switch to grid.
[84:08] No, this is a great stopping point. Yeah, but I really want to echo what Ramon said.
[84:14] Like, we've done a lot on this stream to get you going contributing to DA,
[84:18] and you have made that first commit, you have your first issue,
[84:22] you have that work in progress PR, and, you know, it's open source.
[84:25] Like, we're doing this for fun in our free time after work and stuff.
[84:28] So like, totally fine to pause, put it down, hang out, chat, and then pick it back up the next time.
[84:35] Right? - I'm just gonna say like,
[84:36] if you guys want a guest on your show next week, I'm totally down to go represent.
[84:41] - Please. - Done? - Please.
[84:43] - I love this, I love this. This is the collab.
[84:46] This is the crossover episode. We come into the next season,
[84:50] now you're crossing over on our show. This is great.
[84:53] Also, also, 'cause you said we started a lot, we didn't finish a lot.
[84:57] I would argue gently that we did accomplish something, which was to onboard you onto the code base.
[85:06] This was a successful, well, I hope successful onboarding. I concur.
[85:13] I would say that I need to work on that in general of, just because an overall task hasn't been done
[85:23] doesn't mean that there weren't wins. So thank you, Ramon and Taylor for calling that out.
[85:31] Now, are you guys on the same time zone then? - Yep.
[85:38] Yeah, we are. - Yeah, I'm out with our European team in Belgrade
[85:43] for three months, July, August, September, and then I'll go back to Pittsburgh.
[85:49] So next month or so, I'll be at the same time zone. - Yeah, when I was saying that I was on back-to-back calls,
[85:57] it's because in my 8 a.m. call was with a lot of people in London.
[86:06] And then Kai and I got to hang out a bit at nine, and then we started ours early.
[86:13] So I was like, I am not mentally keeping up, I feel like. I'm like, I need to take time to decongest.
[86:24] There's always so much learning and it's so fun. Now, I do have this question for the two of you.
[86:29] Because tech is encoding, there's always something to learn. How do you keep up with the learning
[86:36] and being open to learning more? - I'd love to jump in if I may.
[86:47] So the question is like, how do you keep up with learning when there's so much learning to do?
[86:52] Is that? - Yes, and being open to it.
[86:55] Because like, for example, with the Python one, it was me comparing so much of what I learned
[87:02] with JavaScript to compare it to Python, which I know is a natural way of learning.
[87:10] We compare it to things we already know, yet that isn't always, Ramon,
[87:15] I'm pretty sure you're the one who told me that's not the best way to,
[87:18] when you let go of comparing it to something. - Yeah, I have thoughts on this,
[87:28] because it's something that comes up a lot with like early stage developers, sorry,
[87:33] emerging developers, which is that sort of pressure to be like, oh, should I learn,
[87:39] like how much JavaScript should I learn before I learn React?
[87:42] Can I skip HTML and CSS before I go into React? Can I go just skip everything
[87:48] and go straight into machine learning with Python and stuff like this?
[87:50] And what I argue to them is like, or what I tell them is like, hey, you know,
[87:56] I know, you know, I can write C, I can, if you give me like a week,
[88:03] I can handle some assembly, but I couldn't possibly look at a processing unit
[88:10] and understand how these additions work. There's always gonna be a deeper level down,
[88:15] and I think that applies to most of the stages of tech, be it, for example, understanding React,
[88:21] but not having any idea what it is that React is doing to manipulate your JavaScript.
[88:25] - Hmm, okay. - There are concepts,
[88:29] and I think the thing that comes with experience is that these concepts do transfer
[88:36] the concept of an array, of a list, of a, there's probably another name
[88:40] for this sort of data structure. - Even the package manager earlier, right?
[88:44] We were using Yarn, and Jen has experience with NPM, and what's the Python one again, Jen?
[88:51] - Pip. - Pip, there we go.
[88:53] And that's a Ramon three or four more out, and so it's like, you have the concept
[88:57] of what a package manager is, and we can include other libraries and frameworks,
[89:01] and it gets downloaded for us to our repo, and we're good to go, right?
[89:05] And so, now that you have that concept down, picking up a new package manager in a different language,
[89:11] it's gonna be kind of the same thing. There might be some configuration details
[89:15] to figure out some documentation to read, but you understand that.
[89:19] Just like how, you know, as you get the concept of functional programming down,
[89:23] that applies to React, where, you know, it's using this sort of, like, run the function,
[89:29] take the output code, shove it into the webpage, right? There's all sorts of, like,
[89:34] purely functional programming languages out there, like Elixir, and so it's like,
[89:41] I think that as you learn, like, the specifics, that never changes.
[89:46] I'm always looking up documentation. I'm always forgetting the stuff I've already learned, right?
[89:50] 'Cause it's been six months since I touched it, or something, you know?
[89:54] And so, you'll get better and quicker at, you know, how do I solve the simple question,
[89:59] or where do I find the docs, or something? Like, how do I investigate this?
[90:03] But you'll start to snowball these concepts, like Ramon was talking about,
[90:07] and then you see something that's in parallel. You don't necessarily need to, like, compare it,
[90:11] but you have that underlying understanding of it, so when you pick something new up, it's quicker, right?
[90:19] - Yeah. Sorry to cut you off there, Ramon.
[90:22] I just, I saw the package manager, like, as a great example of the concept there.
[90:26] - It is, and that's it. I think it's drawing those parallels that,
[90:30] and, you know, I've accepted that in my career, there are going to be things that I don't fully understand.
[90:38] Like, like how to do 3D graphics programming, and like, you know, like, you know, drawing, like doing,
[90:47] you know, it wasn't until I tried out 3D graphics programming that I didn't appreciate the vector algebra
[90:54] that school was trying to teach me. Stuff like this.
[90:59] I've come to accept that I can, I can sort of wrap my head around it, certain parts,
[91:05] but there are things that I'm either going to forget, like Taylor correctly said.
[91:10] I couldn't tell you right off. Jen and I did a stream a few, gosh, was it a few months ago,
[91:16] or at least a month ago? It's been a while.
[91:18] - It was at least a month ago. - So Jen and I did a stream at least a month ago
[91:24] on how to make an ExpressJS server. Here's the thing.
[91:29] I didn't know how to do that by heart. If we were to, if you were to sit me down right now
[91:32] and say, "Ramon, no documentation, let's rewrite it." I couldn't.
[91:36] I couldn't. - No. - And that's okay.
[91:40] - Yeah, I think that's okay. Yeah, I mean, that's why, you know,
[91:42] Google engineers still, Google programming questions, they still ask stuff on Stack Overflow.
[91:48] You know, they just like happen to know a quick and efficient way of approaching that.
[91:54] And I think that's kind of the transition you make is like right now, everything's new to you, right?
[91:59] So it might not feel like you're making a lot of progress, but just like today was like, oh, we did this,
[92:03] and then we did that. You know, it's like once you actually figure it out,
[92:06] because you're trying to learn about everything at once, what ends up happening a bit later on
[92:11] is like you have a solid base that you're comfortable with. You might still have those syntax questions,
[92:16] or, you know, look at the documentation for your library, but, you know, you kind of get it, right?
[92:21] And so then the amount of stuff you're trying to learn at the same time is a much smaller slice, right?
[92:28] And so, you know, right now it's like, it's all new, and it feels like we didn't get a lot done,
[92:31] but actually we did. In the future, it's gonna be like, oh, cool,
[92:34] I'm making like lots of study progress, and then I need to use a new library or something,
[92:38] and let me go, you know, focus on that bit of learning for half an hour or something.
[92:43] Cool, got it, move on. Yeah.
[92:48] - I think that makes a lot of sense, and thank you both for sharing that,
[92:51] and also breaking things down for newbies. It's the type of thing that I've been,
[92:58] until earlier this week, and this is, I was telling Ramon,
[93:01] and I think I was telling both of you this, actually, that I'm really excited because I've been afraid of GitHub.
[93:07] (laughs) - Yeah.
[93:09] - And like how to submit all of this, even though I've been shown a few times,
[93:13] it wasn't until I actually did it for a functional project that I was like, oh, okay.
[93:21] And it's really helpful to start learning this, and also seeing that it doesn't matter how far you get,
[93:30] the shits can still be confusing, we all have to learn. So thank you both so much for this.
[93:36] Is, you know, before we end today, could you both mention how people reach out to you,
[93:43] and also how to connect, or donate, or like follow Distribute Aid, please?
[93:51] - Totally, so if you all can see my screen, I'm @borderless_dev on Twitter.
[94:01] Shoot me a DM, and to contribute to Distribute Aid, like really like check out our GitHub,
[94:07] sign yourself an issue, you know, comment on that. Or shoot me a message on Twitter, and we love sitting there.
[94:14] I think this is like such a great project, especially for people that are still like,
[94:18] you know, starting their kind of dev journey, right? It's a very friendly and welcoming space.
[94:23] And it's something cool that you can contribute to, you know, which you can also put on your website,
[94:29] like, you know, or your resume, or whatever, right? It's like a real thing that does a lot of real world things
[94:36] that you can be like, cool, like I contributed to this project, and that helps get more aid shipped
[94:40] to displaced people around the world, right? Which is, not to say AFD is better or worse
[94:47] than other open source projects, but it does have that sort of aspect to it.
[94:51] Yeah, you can follow us at Distribute Aid, I think on Instagram, Twitter, Facebook, LinkedIn,
[94:58] just Google around for it. And then of course, if you wanna donate financially,
[95:04] much appreciated, we have an open collective for folks in the US, just go to our donate page.
[95:09] $10 a month delivers $10,000 worth of aid by the end of the year, but really no pressure.
[95:15] Like, we're super grassroots and any sort of contribution, even just liking and retweeting the stream next week,
[95:22] which Shen's gonna be on, is a huge support. - Amazing, thank you.
[95:28] - I may or may not have cheekily put some links in the chat. So you can go check out the open collective
[95:35] and the Twitter for Distribute Aid. The photos they post are incredible.
[95:40] Like, it is a series of journeys that are, gosh, what's the word?
[95:45] Overwhelming to follow. It's really magical.
[95:48] So I highly recommend giving them a follow. If you wanna get in touch with me,
[95:52] that's my Twitter handle right there, @HolaSoyMilk. It is a terrible joke.
[95:56] That means, hello, I am milk in Spanish. Yeah, that's me.
[96:02] - Yeah, and hey, Jen, thank you so much for having both of us on here.
[96:08] Like, we've been streaming for a while now and I think it's really cool.
[96:11] Like, I really feel like it's more than just me and Ramon, you know, hanging out, talking about Distribute Aid.
[96:16] So I feel more connected to the larger dev community 'cause you invited us onto your stream.
[96:21] - Yay! And I think I can say that on stream,
[96:27] you are our first volunteer contributor. Is that correct, Taylor?
[96:33] I think it is, yeah. - What do you mean by volunteer contributor?
[96:37] - Like the first one that joins in because and through the stream.
[96:40] - Oh, because of the stream, yeah, yeah, yeah, yeah. - So thank you.
[96:44] - Yay! Well, it's been fun and I look forward to next week
[96:49] and we will get those details hashed out and yay! Goodbye, everyone.
[96:55] Have a lovely rest of your Thursday. For those going to bed, rest well.
[96:59] For those still having your day going, I hope you have an amazing day.
[97:04] Bye-bye. - Cool. 
