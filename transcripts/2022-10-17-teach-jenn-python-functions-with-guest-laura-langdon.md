---
showLink: "https://www.youtube.com/watch?v=tXnW8MNtKq4"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-python-functions-with-guest-laura-langdon"
title: "Teach Jenn Python Functions with guest Laura Langdon"
publishDate: "2022-10-17"
coverImage: "https://i.ytimg.com/vi/tXnW8MNtKq4/maxresdefault.jpg"
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

[00:00] >> Hello, hello, beautiful humans. Welcome to another episode of Learning with Laura,
[00:07] Teach-Gen, Python Tech. That is a very, very long title.
[00:15] But I dig it, I dig it. This is our Python series,
[00:20] and we are going from once every other week to once a week. I'm very excited. We spend Mondays with Laura,
[00:28] it is how the show goes. I like starting every week with you because it's like,
[00:35] I have episodes where I'm just like this goes way over my head, but I know I need to start to understand what it is.
[00:44] But it's like, I don't know what they just said to me. Kubernetes is going to take some time.
[00:52] Go, that one's going to take some time. I dabbled in a bit of Android Dev last week.
[01:01] That was actually pretty cool. We went more through history stuff than going to the development,
[01:13] but I actually got an Android tablet that we are going to deploy an app on Friday.
[01:17] >> Exciting. >> Yeah. But for those who are new to the show,
[01:24] I learned a lot of random tech, and that is why it's called Teach Gen Tech.
[01:30] Good morning, homie. Also, we have been doing this for, oh, goodness.
[01:38] I've had the show for three, almost four months. Lots has been learned,
[01:44] lots more to learn. As I said, Laura is a regular,
[01:48] but Laura, please introduce yourself. >> Hi, I'm Laura. I'm a technical writer
[01:52] at Suborbital Software Systems. I was previously a math professor,
[01:58] and I got into technical writing because I really wanted to keep teaching.
[02:04] Here we are on Teach Gen Tech. >> Yay. Again, I think it's really cool
[02:10] because I actually have this conversation with a friend of mine this morning is when it
[02:16] comes to learning if it's text-based, which coding is, I have a harder time
[02:27] comprehending it compared to talking through with someone. That's a big reason that I started the show is I could do
[02:35] a boot camp or a very structured version of this, but that's not how my mind worked.
[02:43] Luckily, people are willing to come on the show. Yes, Laura, so you know,
[02:49] you can call homie BJ or Ben. >> Okay.
[02:54] >> I've personally stuck with, that's a word, homie,
[03:00] because we have Ben Myers who's on the show a lot. >> Sure.
[03:05] >> I'm like, that's my differentiator. Whatever you would like. I just wanted to read that one out loud.
[03:12] >> Go. No. The dog decided that she wanted to come in and thank you, Ryan. The dog decided that she wanted to come in and join today,
[03:22] and she's been driving me bonkers. If we hear her in the background, my apologies.
[03:30] >> I don't know. I love it when the wildlife shows up. >> That is a good way of saying it,
[03:37] when the wildlife shows up. I dig it. All right. So we are,
[03:45] I need to get back to the right tab, doing a lot today. We have the practice questions from last week,
[03:54] and then we are going to move on to Chapter 3, which is exciting. I was installing stuff,
[04:04] like working on installing stuff, and now this doesn't clear off.
[04:07] >> Oh, okay. I know this one. Control L.
[04:11] >> Control L. Thank you. It was driving me insane.
[04:16] Because I closed it, everything, and it wasn't going away.
[04:21] Thank you for that. I appreciate it. All right. So we talked about Boolean and operator,
[04:32] those operators last week. I have 14 questions to go through,
[04:39] which as Laura has been reminding me, it is not a test.
[04:46] It is, do I remember conversation? Which Laura said there's a really cool way of learning stuff,
[04:54] or remembering, but she wouldn't tell me before the show. >> Okay. Search for Anki, A-N-K-I.
[05:03] >> A-N-K-I. We're going to really hope that this is appropriate. >> It is, 100 percent.
[05:12] >> Anki. >> Yeah. Anki is a way of making your own flashcards.
[05:20] You know what? Maybe I will, if you don't mind, I'll share my screen so I can show you all my.
[05:26] >> Yeah. >> Anki.
[05:28] >> Let's do it. >> Or decks, plural.
[05:32] >> Best way of learning. >> Okie-dokie. So this, and share screen.
[05:45] >> Ryan uses Anki too, as well. Not like 2.0, as well.
[05:51] >> Okay. So this is Anki. Or my Anki deck, anyway.
[06:00] I have a bunch of different, or set of Anki decks, in fact.
[06:03] I have a bunch of different things that I have been working on, or am currently working on.
[06:09] Let's look at my Python deck. This is a deck that I started when I was learning Python.
[06:16] A lot of the questions in here, or prompts in here,
[06:21] come from the book that we're working in, because this is the book that I use to learn Python.
[06:27] If I click study now, so basic code completion shortcut.
[06:32] Then I ask myself, what is the basic code completion shortcut? I have not looked at this deck in a while.
[06:40] I feel like it should be tab, because that's what I would normally do in a terminal.
[06:45] If I were about to type something, then I could press tab and it would finish,
[06:51] it would complete what I was going to say. Then I ask myself,
[06:55] am I sure it's tab? I'm going to go with tab, show answer.
[06:59] It's wrong. It's Control plus Shift plus Enter. I got that all the way wrong.
[07:06] I have four options here where I can rate how accurately and quickly and easily I answered this question.
[07:16] Since I got it all the way wrong, I would click again.
[07:20] If I had gotten it right, but it was like I got it right,
[07:24] but I had to really think about it, then I could click hard.
[07:27] Then good and easy are like good is, yep, I got it, and easy is like, yeah,
[07:33] it was just right in my cognitive muscle memory. Since I'm going to say again,
[07:43] so one card studied in one minute. Right now down here,
[07:48] we've got 0 plus 1 plus 19. That's going to add to 20 because that's the number of cards I've told Anki,
[07:56] I want to review in a session. This is one is red because I had one wrong,
[08:04] and 19 are green because the last time I answered those questions, I got them right. Then you just keep going through this process.
[08:13] If you answer a question correctly, then the next time it'll ask you again in one day.
[08:27] If you get it right again in one day, then the next time it'll space it out to three days,
[08:32] and then it'll space it out further. It's coming back to that spaced repetition that I think we've talked about before.
[08:38] This is like the grandmother of spaced repetition. This is spaced repetition structured.
[08:52] >> First off, thank you for showing this because this is something that I am pretty sure I've told you,
[09:00] but if not, I want to say it again. Thank you for always teaching me the ways of learning too.
[09:06] That's something that I really, really struggled with in case anybody wanted to know.
[09:12] I technically dropped out my senior year, but my mom went bananas in the fact that she was like,
[09:22] "You went through all this summer school, how could you do this?"
[09:25] She convinced the school that I had enough credits to graduate, which I feel very fortunate for,
[09:30] but I graduated with a 1.66 GPA, like straight Ds, basically.
[09:39] I say that in the fact of I never learned very good studying, habits, so my mind would have never gone to this.
[09:50] Never in a million years would have thought of this. I've never understood flashcards in the fact of,
[09:58] I think with what we're working on right now, it has the questions,
[10:02] so I could go put those questions in there. Yet at the same time,
[10:08] if it was just like, I don't know,
[10:12] building a React app with Beat and Vercel, I was like,
[10:19] "What would I put in there to remember stuff?" Now, I know who to bug later on.
[10:29] It gets way cooler than what I just showed you too. It's so powerful.
[10:33] You can put all kinds of different stuff in there. You can put in, when I set this up,
[10:37] I wasn't proficient in Anki, so when I set up that Python deck,
[10:41] because that's like my very first deck, but my newer ones have...
[10:46] You know what? I'm just going to show you,
[10:49] even though this is not a thingy scream. - It's a learning with Quora.
[10:54] It's a learning with Quora. - Thank you, yes.
[10:56] Thank you for reminding me. - Yeah, this is just a learning with Quora thing.
[11:01] That is what it is. - This Vim deck is a more recent one for me.
[11:06] It shows up with this box that you can actually type in, which is what makes a lot more sense.
[11:14] If you're trying to learn syntax, you don't want to just think it,
[11:19] you want to type it, because you want to get that connection,
[11:24] neurological connection into your fingers for what you need to type for this.
[11:29] This is substitute new for old globally, and that would be,
[11:35] we need mod S. Actually, we probably need a colon first.
[11:40] Mod S, new, old, G for globally.
[11:48] Okay, and then I'm going to... Oops.
[11:51] And so you can actually type it in, and it'll let you know.
[11:56] - It does show you. Oh my gosh, this would have been so helpful with math,
[12:00] because this is before I knew I was dyslexic. So I would be doing the problems properly,
[12:06] but I would put the period in the wrong space, or the wrong part of it,
[12:12] or where this is really cool, because it shows the two,
[12:19] and what you did correctly, and what you didn't do correctly.
[12:22] - Yeah, so this is, I actually use this command all the time,
[12:26] so I got it wrong on purpose, so that it would show us stuff that was wrong.
[12:32] So what it's saying is, hey, look, you didn't put in the, what was wrong?
[12:38] Oh, I had a dash here where I shouldn't have had, and I swapped the new and the old.
[12:50] So it'll actually show me. So then I can say like, again,
[12:53] or if I know, because this is all about you writing your own knowledge,
[13:01] right? Somebody else is not looking at this.
[13:04] Somebody else is not grading you. So if you know that you just had a typo,
[13:08] and you know this thing, you don't have to say, oh, I got it wrong.
[13:12] 'Cause I know, 'cause I use this all the time, that I know this.
[13:15] And so instead, I'm just gonna say, good. And then it'll ask me again in like some number of days.
[13:24] You can also do it with like music files. You can put in images.
[13:30] - Oh, that's so cool. - It is incredibly powerful, ridiculously powerful.
[13:36] So anyway, that's Anki. And that is what is really being,
[13:45] it's been really integral to my learning. And some days or some months, in fact,
[13:51] you have bad months. And so then you go back to it,
[13:55] and you just have to click like again, again, again, on like all of them and so on.
[14:00] And you can just pick it back up. And it'll learn like, oh, okay, you forgot these things.
[14:06] So now I'm gonna go back, I'm gonna bring it back. Instead of asking you again in six months about this thing,
[14:11] I'm gonna ask you tomorrow. - How much time do you just like do 20 questions?
[14:19] Or do you do X amount of time per day? Like these are things I overthink about, but.
[14:26] - I mean, it's totally up to you and like what your goals are.
[14:28] So when I was first starting out, and there was just a ton that I needed to learn,
[14:34] I would set a time goal. Now it's more of a number of cards goal.
[14:39] Because I can go through the cards super fast. So I don't need to spend 20 minutes a day on cards,
[14:48] because I'd be going through hundreds and hundreds of cards. But you can, oh, and like Ryan says, you can customize.
[14:56] Like, I wanna see this many of cards per day from this deck, but I wanna see, I only want five cards a day
[15:02] from this other deck, because this one- - Oh, so it can mix decks.
[15:06] - Oh, yes. - Wow.
[15:08] - Well, you see one deck at a time. - Okay.
[15:11] - But you can customize the settings per deck. And like the number of review cards
[15:17] versus the number of new cards. So I used to set mine at like 20 new and five review
[15:23] was like my default. But then for some decks, I'd be changing that up
[15:28] and like, okay, I want more new cards and so on. - Okay, y'all, this is like the coolest thing ever.
[15:36] And it also has, you can download it for iPhone and Android too,
[15:45] which I'm pretty excited about because we just got the tablet too.
[15:49] So that way I can do like the Android dev stuff. So like, this is another use for the tablet, yay.
[15:56] - You can literally be standing in line at Costco doing your Anki cards.
[16:02] - Interesting. Yay.
[16:10] - And thank you, homie. I did, he said more motivated to help Jen reach her goals.
[16:18] Let's go. - Yes.
[16:21] Thank you, it is definitely learning. It's people, it's kind of crazy
[16:28] because like just as like a side note and I really want to iterate this for like everyone
[16:34] is a lot of people don't realize that I'm not great at learning because I'm very perceptive
[16:41] and I can pick things up very, very quickly because like just because of that.
[16:47] But when I don't know something, I really, really don't know it like at all.
[16:52] Like cameras, it sounds really weird, but cameras and I, I still don't understand like F-stop
[16:59] and, you know, exposure. Like I've taken multiple camera classes.
[17:04] I intern at a videography production studio and it just never, ever clicked.
[17:12] And I think a lot of it was not being able to do it repetitively to really learn it.
[17:18] And also in a language that I could learn it in. So thank you.
[17:25] Like, this is like mind blowing to me. - Right.
[17:28] - So. - Yes.
[17:31] - Bananas, bananas. - Oh, and I'm so glad that my hand gestures
[17:36] aren't distracting 'cause I worried that they were going to be.
[17:40] And then I was like, you know what? I just, I gotta be me and the hands,
[17:44] they're just gonna move unless I like tie them to the chair.
[17:46] So. - I do hand gestures.
[17:49] I like flail, flail, which I find this very interesting. Just as a random side note for y'all,
[17:58] this is the, a Taekwondo sweatshirt from seventh or eighth grade.
[18:08] Like the shirt is over 20 years old. And so I find it really interesting
[18:14] that we're talking about school and I'm wearing this shirt.
[18:17] It's like, whoa, so cool. Bananas.
[18:21] All right, so Anki needs to be bookmarked really quick. And I also like the idea
[18:30] because what I'm gonna be doing next is the CLI commands. And so to do that, I'm looking at it again.
[18:43] And I like how I could even do this to remember the CLI commands.
[18:51] So. - Yeah, yeah. I have a git deck.
[18:55] - Okay, so I want to clone, clone. No, that's a gist.
[19:06] Core commands, authorize, browse, gist, issue. - Yeah, release, workflow.
[19:14] Did it the other day. - So this is to use the GitHub CLI, right?
[19:30] - Yeah, 'cause I was gonna open the project, like clone it and.
[19:35] - Why? And you probably have a good reason for this.
[19:40] So this is not me being like, I think you do not have a good reason for this.
[19:44] This is me wanting to know your very good reason for using the GitHub CLI instead of git.
[19:50] - Probably because I've gotten used to using. - My headphones just disconnected, one second.
[20:05] I don't know why they do this all of a sudden. Come back.
[20:11] - No, I could do it this way. - Okay, we're connected, sorry.
[20:15] - You're good. I think it's because I've,
[20:20] I learned command line back before I started on all of this. And if I'm gonna have to use command line for some things,
[20:28] I'm just trying to put all things that could be in command line in there.
[20:32] So that way, when people ask me about it, I'm more used to it.
[20:37] - Git does happen in the command line. It happens in your terminal,
[20:43] which is a command line interface, a CLI. - Okay.
[20:48] - GitHub has its own command line interface. - And I've installed that.
[20:55] I just didn't know, 'cause like, well, what I was gonna try to do,
[21:02] and maybe I'm making it way too complicated, which I may be, let me make it up, there we go,
[21:09] is I know that I'm gonna do something that will let me go to code,
[21:17] command, oh, I can't. - Oh, okay.
[21:21] - That's what I'm trying to do. Is this, this right here, this is what I'm trying to do.
[21:26] - Click the HTTPS tab instead of the GitHub CLI tab. And you can still use that button,
[21:32] but you can just use straight up Git instead of the GitHub CLI.
[21:37] So here you can, yeah, mm-hmm, go ahead. Although in fact,
[21:54] you don't actually need to make a directory first, because it'll make one for you
[21:59] with the same name as the repo. So you can just type git clone.
[22:07] - Okay. - Space, paste that link.
[22:12] There you go, enter. - Oh.
[22:16] - And now do an LS. And what you'll see is you've got
[22:20] that learning Python repo cloned. So the GitHub CLI, I would say is probably like,
[22:31] now I have not used it. So I am wildly speculating here,
[22:35] but I think it's probably, I'm not sure why they made it.
[22:44] So like there is a use case for why you would use the GitHub CLI
[22:47] and just instead of just your straight terminal. In my experience,
[22:52] you're more likely to be using the terminal than you are the GitHub CLI.
[22:56] And apparently the commands are different. And all the commands that you're gonna find
[23:02] in like stack overflow and like all of the stuff when you're trying to figure this stuff out,
[23:06] they're all gonna be git, not the GitHub CLI commands. And so I think that git will get you farther
[23:14] than the GitHub CLI. So my bias is toward, let's just do straight git.
[23:23] - Is there then on that note, so I would just look up git CLI?
[23:35] - Git is a command, like it's a language that you use within a command line.
[23:45] So you would just look up like git commands. And I have a favorite resource for this.
[23:51] Learn, let me see. I love how we're like 24 minutes into this
[24:00] and we haven't started the Python yet. And that is okay.
[24:03] - This is, I'm not gonna lie. This is a big reason I really appreciate
[24:07] doing this stuff with you, Laura, is this is like my,
[24:10] it's weird to say like a safe space to do like really, really basic stuff.
[24:16] And it's like, I don't, and I wanna say like, I do wanna call it out.
[24:23] Like I don't feel dumb asking questions to everyone, but you really pick up when I need the basics first.
[24:32] Not everybody is able to pick that up. So I really appreciate that.
[24:37] On Mondays, I'm like, you're helping me build good patterns,
[24:40] not just teaching me the, to learn the tech, you have to build patterns,
[24:46] to build the patterns. A lot of people already know them.
[24:51] I don't know them. So you really helped me break them down in,
[24:56] and then also check on me and be like, yo, yo, did you do this?
[25:01] Do you remember? So it's been really, really helpful.
[25:05] So I do, I agree. I'm like, this is good stuff and it's important.
[25:08] So I appreciate that. Y'all think that too,
[25:11] because this is what I think a lot of newbies don't necessarily, she is a permanent Monday guest.
[25:17] - Yep. Already established.
[25:21] - Yep. She didn't know this when she started.
[25:26] She was going to come on once, and then I convinced her to every other week.
[25:30] And then as of last week, she said she would come on weekly.
[25:34] So yes, she's a permanent Monday guest. - Yay.
[25:38] - I love being able to start Mondays with Laura. - This stuff that we're talking about
[25:45] is actually content in an MIT, I think it's online only CS course
[25:50] called The Missing Semester, where they actually teach you,
[25:54] like get and commands at like terminal commands and things like that.
[25:58] So the, what we want to do is I'll put the link in the private chat, I guess,
[26:03] 'cause I just realized I can't put it in the thingy. Come back.
[26:11] Here we go. Learn git branching.js.org.
[26:17] This is my safe space for fucking around with Git
[26:26] and figuring shit out. And so it'll actually show you what,
[26:34] like literally show you what's happening with different Git commands.
[26:41] And you can then put these into your Anki deck, your Git Anki deck, that is.
[26:51] Hold on, we have to do a new bookmark folder. You get your own folder.
[27:06] - That's exciting. - And yeah, it's good to go.
[27:10] - I rank with D&D, I noticed. - Yeah, yeah.
[27:15] - Yeah. So I feel special.
[27:18] - Because you're on here every week. So you gotta, I can put stack overflow,
[27:24] I haven't used it yet. But yeah, you're on here every week
[27:28] that it's something that it does really, oh, this is kind of fun.
[27:33] - Yeah. - I will be distracted by this all day.
[27:38] I will close that. We got it open.
[27:41] There we go. Okay, let us go to the Python.
[27:49] - And these questions too, you can put in your Anki deck later.
[27:54] - Okay. And maybe that's how we will do next week's
[27:59] is I'll have it in the Anki deck and we could do them all.
[28:02] We'll just do a quiz week for the first three weeks. See if I can figure it out.
[28:08] Okay, what are two types of Boolean data type? What are the two values of the Boolean data type?
[28:18] How do you, do you write them? I believe true and false.
[28:24] - Correct. - How would I write them?
[28:27] I don't know, is it-- - So it's a little bit like when I read this,
[28:44] I'm like, okay, do you mean, and when you say, how do you write them,
[28:48] do you mean like literally how do you type T-R-U-E? And I think yes.
[28:55] And I think that the question would be, is it a capital T or a lowercase T?
[28:59] - Oh. - That's what I can come up with
[29:03] for what this question is trying to ask me. - Okay, because I like in my mind,
[29:07] I'm like, it's an uppercase T or an uppercase, like the first letter is uppercase.
[29:14] It could be, I literally don't even remember. So this is the kind of thing where I have to,
[29:23] I have to go back and like check things like that because it's tricky in my brain.
[29:30] Yeah, it is lowercase. It'll, oh yeah, yeah, okay.
[29:33] This is why it goes in my head. So when you type it, you have to type it with a capital T.
[29:40] When it gets returned, it's a lowercase T. - Yeah, that's not confusing at all.
[29:46] - Right, that's why I was like, no, 'cause I can literally, I have sort of a visual memory
[29:51] and so like I can literally picture it with the capital T and I can picture it with a lowercase T.
[29:57] Why can't I picture both of them? - That makes more sense though, okay.
[30:01] So what are the Boolean operators? Which you guys might've just seen, I was on that one.
[30:09] I was like, oh, wait, I should. I feel like it's greater than, less than,
[30:16] or one, equal to, and not equal to. - So those are the sort of mathematical operators,
[30:29] but they're comparison operators. - Okay, oh, so it's number five.
[30:36] I'm thinking of number five then. - Mm-hmm.
[30:39] - Okay. - Yep, yep.
[30:41] - What are the three Boolean operators? And, or, and, or. (laughs)
[30:51] - What is the remaining possibility? - And, or, not?
[30:59] - There you go. - Oh, yay. (Molly laughs)
[31:05] - Write out the truth tables of each Boolean operator. That is every possible combination of the Boolean values
[31:13] for the operator and what they evaluate to. - This is the kind of thing that is way super fun for me.
[31:19] We didn't actually go over the truth tables. - Should we go look at them?
[31:26] - Sure. It's a little bit like a multiplication table
[31:34] in the sense that it shows all the possible combinations, like all the possible values
[31:39] of all the possible numbers or whatever. - Okay.
[31:42] - Yeah. So I think what he's got here
[31:49] is the truth table just for the or, but you can have one for and, and you can have one for not,
[31:55] and all the combinations thereof, and so on. - Okay. - So, yeah.
[32:03] So I'm just thinking if I do, these make sense, the or ones.
[32:15] Oh, there we go. And ones were right above it.
[32:18] - So the thing that we need to know is that for and, both, so these are binary,
[32:30] and and or binary operators, because you have to be comparing two things to each,
[32:34] or yeah, comparing two things to each other. So if they are both true, then and is going to be true.
[32:42] And this works the same way like in colloquial English. If you would say,
[32:51] today is October, what the hell, 17th, and today is Monday. If that's a true statement, right?
[33:03] But if I said today is October 17th, and it's Tuesday? - It's false. - False.
[33:09] - Yeah. - Because they weren't both true. - Today is October 17th, and my mom's birthday.
[33:15] - Happy birthday, Jen's mom. - Yay, and that's true.
[33:19] - If we scroll down for or, only it's at least one of them has to be true.
[33:29] They can both be true, but at least one of them has to be true.
[33:33] - Yeah, and I think that's the confusing part, is if it's true or false, why are they true?
[33:43] - So it does work the same way in English. So like you would say,
[33:55] if like, so you're going to the grocery store, pick up some, you know, depending on what's in stock,
[34:05] pick up some coffee or pick up some tea. - And I guess where my head would go would be,
[34:14] what if they're both in stock? - Sure, and then maybe that would be like,
[34:19] you pick up both potentially, but because both are true, but like at least one of them has to be true,
[34:25] or like at least one of them is in stock, you know. That's not a very good example.
[34:35] - No, I think just like how you just said it of like, if kind of like, if they have coffee, get coffee,
[34:47] or if they're out, get tea. - Yeah, and so then when the person comes back,
[34:54] if the coffee was in stock, they'll have the coffee, or if the tea's in stock, they'll have the tea.
[34:59] So both of those are true. If neither of them were in stock,
[35:02] they come back with nothing, which is false. - Okay, that makes sure.
[35:08] That makes sense, that makes sure, that makes sense. And then, okay, the nots totally make sense.
[35:16] I didn't realize that not was actually the answer. Because it's so intuitive that we're like questioning it.
[35:26] - Yes, yes, so this one is, so not true is the opposite, which is false,
[35:37] and not false is the opposite, which is true. Yay. - Yay.
[35:40] - Okay, so that was number two, and number three, cool. What do the following expressions evaluate to?
[35:51] Thank you, Bakari, and thanks, y'all. Yeah, I already called her, I FaceTimed her.
[35:59] Don't worry, I did call. In case everyone's curious,
[36:03] I'm really bad at actually mailing birthday cards, cards in general, just physically.
[36:09] So half the time my mom doesn't get one, which she loves birthday cards,
[36:14] so last night I'm sending her a video of I'm like, mom, it actually is going in the mailbox
[36:21] before your birthday, technically. Granted, it's Sunday, you'll get it afterward,
[36:25] but it's in the mailbox. So she was very excited about it.
[36:31] But thank you, Bakari, as well. So five is greater than four,
[36:38] and three is not five. Not five?
[36:49] I don't remember what this one means. - Is equal to.
[36:52] - It is equal to. Then what's the difference between
[36:55] the one equals and two equals? - So one equals is assignment,
[37:03] and so you can read it as like gets. - Oh, so like if you do like true equals five,
[37:12] that's an assignment, or five equals true or something. - Neither of those would be allowed, particularly,
[37:19] because like you can't say that five is, 'cause five is a thing in Python, right?
[37:25] But you could say like a variable x equals true. - Okay, okay.
[37:30] So then that would be false, because three does not equal five.
[37:40] - Right. What if it had been an or, instead of an and?
[37:44] - It would still be false, because three still does not equal five.
[37:52] - So what's the difference between and and or? - It would be true, because with or,
[38:01] its default is true if one of them are correct. - At least one.
[38:05] - At least one. So yes, one would be, yeah, okay.
[38:10] - There's something else. The reason that I keep harping on the at least,
[38:13] at least one, is because there's another operator called an XOR, which is exclusive or,
[38:19] which means it can only be one of these. - Okay.
[38:24] - But or is at least one. - Okay.
[38:28] Not five is greater than four. False, because five is greater than four,
[38:41] and it's saying that five is not greater than four. - It's negating the value, the truth value
[38:51] of five greater than four, yeah. - Okay, and then five is greater than four,
[38:58] or hey, we changed it to or, so this one's true. - So we've done that one.
[39:02] - Yeah, not five is greater than four, or three is equal to five.
[39:09] - True, because one of them is correct. - So what's the difference between line four
[39:19] and line five there? - It's saying that one of these are negate, is negated,
[39:28] and so three is not equal to five, so therefore that not is true.
[39:35] - Okay. - So in fact, what it's doing is,
[39:40] check out the parentheses. This is where I like working in an IDE,
[39:46] not that that would change it, 'cause this is a book, but the IDE, like I like to use rainbow brackets,
[39:53] 'cause it'll color, so I can tell the difference between my nested brackets.
[39:57] So what it's negating is everything that's inside of the nested parentheses.
[40:05] - So it would be false because it's inside the entire parentheses, not just one or the other.
[40:11] - Yeah, so what's inside the entire parentheses is the same thing that's on line four,
[40:16] and the truth value of line four is true. So we're doing not true.
[40:23] - So it would be false. - And true and true, and true is equal to false,
[40:34] so this would be false. - That's correct.
[40:37] - And not false or not true, that is true, because it's an or.
[40:44] Because it's true or false, and on all the true or falses, they were true.
[40:51] - Yeah. - What are the six comparison operators?
[40:59] Oh, I was mentioning these earlier. Greater than, equal to, I don't know,
[41:07] less than, is that compared? - Sure.
[41:16] - Compared to a different one? - Right, we got greater than and less than.
[41:18] - Okay, equal, double equals, or would assignment be one of them?
[41:26] - So it's double equals, but not equals, because assignment isn't comparing something,
[41:33] it's assigning. - Okay, so greater than, less than, double equals,
[41:37] I'm just saying that so that way I remember it. Greater than, equal to, less than, equal to,
[41:45] not equal to? - Got it.
[41:50] - And the not equal to is the backslash equal, right? - It's exclamation point equal.
[41:58] Bang, equal. - Where'd it go?
[42:04] I'm gonna look at it. Come on, you gotta have like a chart or something.
[42:10] - We could maybe do a control, like a command F, like a find in page for search for like not equal.
[42:20] - Oh, not equal, yeah. Oh, there we go.
[42:25] Okay, cool, cool, cool. Yay.
[42:29] All right, so, and we're gonna get through the quiz. Explain what a condition is and where you would use one.
[42:51] - If George is yellow, then. - There you go.
[43:01] - It would be true. - Yeah.
[43:03] - If George is orange, that it would be false. - Sure.
[43:09] - So it's like, if we could see George. - The word that you said first.
[43:16] - If, yes. And you would use it in the charts we were making of if.
[43:25] - You can use it in code too, right? Like we wrote some if statements.
[43:30] - Yes. Okay, identify the three blocks in this code.
[43:49] - I feel like this is gonna be cheating though if I bring it up for, like if I copy this and put it,
[43:56] because it will tell me, it'll give me squigglies.
[44:04] Oh, it actually pasted it. Did it paste it the same way?
[44:09] - Yeah. - Okay, so blocks of code.
[44:18] Wouldn't it be like, this is a block of code and this is block of code
[44:22] and then the first one is a block of code? - Yep, every time you have to indent, you're in a new,
[44:32] well, yeah, every time you've got like nested indentations, you've got new blocks.
[44:39] - Okay, so it would be a block within a block within a block. - Sure, yep.
[44:46] And that's kinda what we have going on here because we have nested if statements.
[44:51] 'Cause the first thing that we look at is if spam is equal to 10, then we're gonna print eggs.
[44:56] And then we're going to go into a new if statement within the outer one.
[45:01] These are the Matryoshka dolls, right? - Yes, yes.
[45:07] And Ryan, you definitely have a point. Does it matter?
[45:10] No. I still like, so when Laura and I first started recording,
[45:15] we talked about like the stigmas and fear that goes into learning and specifically math.
[45:24] And so when I'm like, yeah, it's definitely, and this is why I appreciate that Laura does this,
[45:31] is it's like finally undoing a lot of that. - It's like that, you know, that feel the fear
[45:39] and do it anyway? - Yes.
[45:42] - When I first heard it, felt sort of condescending. Like, okay, it's scary, but you just have to, whatever.
[45:49] - Yeah. - But what it says is feel the fear.
[45:52] It doesn't say ignore the fear. - As my mom does not like me saying it,
[45:57] it's my term, fuck it. You feel it, you don't wanna do it, just do it anyway.
[46:02] And for all of those, we finally got the dog to calm down. So you may hear her randomly snoring in the background.
[46:11] Oh, that's the best. She is, she finally went to sleep, which is good.
[46:17] So if you hear snoring, it's her. All right.
[46:22] Write code that prints hello if one is stored in spam, prints two if howdy is stored in spam,
[46:30] and three prints greetings. Wait, isn't this what, ah, where does my, there.
[46:39] Ah, I think we just did this though. Write code if spam, if-
[46:49] - Can you scoot your IDE over and the browser over so that we can see the-
[46:56] - I just typed it in for line nine or line 33. - Oh, gotcha, sorry.
[47:02] - But let me make this bigger because it's even small for me and I'm staring at the big screen.
[47:07] So there we go. Okay, but I like your idea better.
[47:20] I thought my idea would work, it didn't, so. - I'm looking at the comments and Ryan says,
[47:29] exclamation, so Laura, and I literally don't know what that means.
[47:35] - Ah, I think it's shout out, but I need a setup. So y'all, something that I'll be doing this week
[47:42] is setting up OBS and working on some screenshots for show my.chat for Hacktoberfest,
[47:53] because since I finally got my proper GitHub name, the two Hacktoberfest PRs that I had are null and void.
[48:05] So I have to, yeah, I have to get a few more, I have to get four PRs.
[48:10] So I got to hurry up and do that and to do that. So I think like the exclamation SO
[48:18] or like they did some earlier exclamation stuff, like clap is if I had OBS set up,
[48:26] it would clap on the screen. - Oh, okay, okay, gotcha.
[48:34] - Y'all let me know if that's. - 'Cause I was literally reading it like Python code.
[48:41] So that would be like, not, not shout out Laura. And I was like.
[48:46] - No, they love you. - I'm sorry, did I do something offensive?
[48:53] Gotcha, okay. - Yeah, so, okay, well, yes, shout out to Laura.
[49:04] - All right, so write code that prints hello if one is stored in spam, prints two if stored in spam
[49:12] and prints greeting if anything else is stored in spam. So I feel like it's like basically this,
[49:26] but prints hello, okay. Okay, hello if stored in spam.
[49:37] So, 'cause if I do spam equals zero, then it means that it could equal anything, right?
[50:03] - No, it means it's zero. - I'm gonna leave that blank for right now.
[50:12] If spam equals one, equals one. If spam equals one, equals one.
[50:22], print hello. If spam equals one, print hello.
[50:32] If spam equals one, print hello. [50:35], print hello.
[50:40] If spam equals one, print hello. If, if, if, oh, if spam equals one, equals one.
[50:51], if spam equals two, equals two. If spam equals two, equals two.
[51:01] If spam equals two, equals two. If spam equals two, equals two.
[51:13] If spam equals two, equals two. Cool.
[51:16] (sneezes) (sneezes)
[51:21] (sneezes) (sneezes)
[51:26] (sneezes) (sneezes)
[51:30] (sneezes) (sneezes)
[51:35] (sneezes) (sneezes)
[51:39] - I feel like I'm missing something. - That's okay, because we can, we can,
[52:09] we're going to iterate until we get to where we want to be. Right?
[52:14] - Right. - What we did was we got past the like blank page problem.
[52:17] We got like stuff. We got some code down and now we can like.
[52:23] - I'm going to make it that way. I can only see this one.
[52:25] I guess I could just run it. This one.
[52:29] - And see what happens. - Yeah.
[52:34] I feel like there should be a way to do this that would be sort of similar to a Jupyter notebook
[52:39] where you can like execute just that. - Area?
[52:44] I can make a new page, I guess. Just, it'll get me practice on.
[52:49] - You know who would definitely know the answer to the question that I just asked as a statement is.
[52:57] - Jay. - Jay, right?
[52:59] - Jay. Where's Jay?
[53:02] - We're just going to call this bam.py. And voila.
[53:08] - Cool. - And is this the run?
[53:12] Run Python file. Oh, yeah, no.
[53:19] - Why not? - Cause it did everything.
[53:24] - Why did it do everything? (sniffles)
[53:30] I feel like that, but I don't know. If spam equals one, print hello.
[53:49] Would it be two different? - Did it do everything?
[53:55] - Huh? - Did it do everything?
[53:57] - Oh no, it didn't do howdy. - Right.
[54:06] - Oh, because I need an input? - No, your input was fine.
[54:11] So your input was one, right? Okay.
[54:14] So let's look at what it's going to do line by line. - Okay.
[54:17] - Okay. So what's happening on line two?
[54:20] - If spam equals one. Oh, I need a input spam.
[54:25] Like I haven't asked people to put spam in, right? - You don't have to.
[54:31] - Okay. - You've declared a value for spam.
[54:34] So if spam is equal to one, then what's it going to do? - Print hello.
[54:40] - And then what's it going to do? - If spam equals two, print howdy.
[54:52] And then everything else, print greetings. But spam can't equal one and two.
[55:00] - That's true. You'd have to change the declaration
[55:06] of what spam is somewhere in there. Okay.
[55:12] So then why did it print greetings? - I don't know.
[55:22] - 'Cause this is a nested if statement, right? We've got if spam is equal to one,
[55:34] we're going to print hello, and then we're going to check and see if spam is equal to two.
[55:41] If it's equal to two, then we're going to say howdy. And if not, we're going to print greetings.
[55:48] So you declared spam to be one. So in line two, the computer said, okay,
[55:54] if is spam equal to one? Yes, it is.
[55:57] So given that that was true, I need to print howdy. Then I need to check, is spam equal to two?
[56:03] Well, no. So we're in the else, and we're going to print greetings.
[56:08] So then what happened? Is that your second if statement
[56:18] is in your first if statement? - Oh, so it shouldn't be nested?
[56:26] - That's right. And you know what you can do when you need to move,
[56:37] change the indentation of a bunch of lines at the same time, you can select them all and press shift tab
[56:44] to move them all back at once. - Sniffles.
[56:52] So would it be or if spam? - Let's look back at the question statement.
[57:12] Okay, so it's supposed to print one or hello if spam is one, and it's supposed to print greetings
[57:25] if anything else is stored in spam. So the else, if you look at your code,
[57:31] the else is associated with which if statement? - The first one, and it should be associated with both?
[57:43] - It's actually not associated with the first one. It's associated with the second one.
[57:52] The first one has no else statement. - Oh, oh.
[57:58] - So what we can do instead of doing two if statements is remember there was something else we had if,
[58:09] and we had else, and there was a third option. - If else or if allow.
[58:14] - Else if, else if. Yeah, exactly.
[58:17] - Hello. So how does it, but if I don't have like an input
[58:36] of what to type, wouldn't I need an input of what to type to make it work?
[58:42] - You declared on line one that spam was equal to one. - Oh.
[58:47] - So you could change, you could put like a loop in there so that like it can get user input, but you don't have to.
[58:54] Yep, you can do that, sure. - Okay.
[59:00] Wow. - I think you should need parentheses after the input,
[59:11] like an open and closed, because input is a, it's a function. So in Python, you don't usually split up your string.
[59:28] Your brackets, like you do in lots of other languages, they usually stay on the same line.
[59:34] - Yeah. I just wasn't typing in the right area.
[59:43] - There you go. - Oh no, you just did it, and now you're not doing it.
[59:54] This is, ah. - It wasn't 'cause of the space though.
[60:02] I think you just hadn't pressed run again. It doesn't need a space in input.
[60:08] It doesn't hurt it, it's fine, but it doesn't need it. - Okay, so one.
[60:15] - No. - One.
[60:18] Still found my greetings. - Okay.
[60:24] - Um. So what's going on here?
[60:28] Did it? What is the problem here?
[60:38] - Ah, the Frank Freeman said this might actually be a different kind of issue.
[60:44] - You know what? Put below line one, put a print spam.
[60:57] Print parentheses spam. And let's just see what's getting stored in spam
[61:06] to make sure that that's correct. Oh, wait, are you saving in between before you run?
[61:19] - Yeah, I was, but I. - Just making sure.
[61:23] - This has one unsaved. I don't wanna save.
[61:26] Well, I could just, like, I just hit save, save. It keeps saying one unsaved.
[61:36] - I think it's actually the lorescool.py that it's considering unsaved, maybe.
[61:41] - There we go. - Okay, so go ahead and press an input.
[61:49] (mouse clicking) Or sorry, enter an input in your, like, run your program,
[61:56] and it'll prompt you for the input. There you go.
[61:59] And now it should, okay. So it's printing one.
[62:03] And so why is it going to readings still? So let's see.
[62:09] So if spam is equal to one, we're gonna print hello, else if, and then else.
[62:15] So why is it not printing hello? Oh, oh, oh, you know what?
[62:21] I think that the else if and the else are supposed to be indented.
[62:27] - Oh. - There you go.
[62:30] - And Ryan said, "I believe to know why it always runs the else branch.
[62:41] I'm not sure if I should tell you why yet." - Not yet, thank you for asking.
[62:47] Yes, okay. - This one, oh, it doesn't need to be as indented, right?
[62:53] No, I just redid that. - Ooh, yeah, yeah, yeah, do the view problem.
[63:04] 'Cause this is a really good skill to learn. - Okay.
[63:08] Hint, the data type of the return value of input. - Yeah.
[63:30] So what, when we type one, so this is a really sneaky thing.
[63:39] And that's why I like, I didn't even, I didn't catch it at first.
[63:44] When we enter the one, what kind of input, oh, you know what?
[63:48] Okay, this is a totally good skill. So this function is input that's part of Python, right?
[63:56] Let's look up what this function is going to return to us. So we can, do you have,
[64:07] what happens if you hover over input? There we go.
[64:14] - Oh, it doesn't have a string or a integer. - It's going to return us a string.
[64:21] See how like at the end, it's got like red arrow and then STR? It's gonna give us back a string.
[64:26] So we said, we're looking for the number one. But what we type in is going to come back as a string.
[64:36] So what's coming back is the string one. - Oh.
[64:43] - So how can we, and this is something we've done before, we like, you can cast a spell
[64:51] to turn something into something else. And it's literally called casting in programming languages.
[64:56] We can cast something as something else. So we don't want this to be an integer.
[65:02] We want to, or sorry, we don't want it to be a string. We want to cast it as an integer.
[65:07] So we need to cast the integer spell on our string. So we can nest that input function
[65:21] within the integer spell function. And then how do we abbreviate integer in,
[65:34] well, most programming languages, but specifically in Python.
[65:37] And that's a function. And so it needs to have parentheses.
[65:44] So you would delete the space and then, yeah, and then put your closing parens on the other end.
[65:52] There we go. And now if we rerun this, we're gonna be good
[65:57] because we have cast it, cast our string as an integer, which is what we were looking for.
[66:03] Yay. - Oh wow. - So that technique of hovering over a function
[66:19] so that it can tell you what it wants you to give it and what it's going to give you is really helpful
[66:27] for this kind of problem where you're like, I'm looking at this code.
[66:30] And as far as I can tell, this fucker should be right. And then you can look at it and be like, okay,
[66:37] so if it's not right, then that must mean that you're returning something
[66:40] that's not what I'm expecting you to return. Please tell me what you're gonna return.
[66:45] - And thank you everyone for also only doing hints instead of giving it away.
[66:52] Granted, I sometimes hate making these mistakes live because I feel like I'm dumb for doing it,
[67:00] but yet I really appreciate everybody's help and especially Laura being so kind as I'm doing it too.
[67:08] 'Cause I'm like, okay, this is why I'm doing these live streams.
[67:12] This is why. - This is the kind of thing though
[67:15] that happens to everybody. Even if you've been doing it forever,
[67:21] like I've been writing Python for a long time and I didn't catch it right away.
[67:26] - Yeah. - Well, a long time. - Bye Ryan.
[67:28] - I've been writing Python for two years. Bye, thanks for joining us.
[67:32] - Yeah, I think it's definitely something too where it's just like,
[67:35] it's hard to make the mistakes in public so much, but thank you.
[67:39] Thank you for, ooh, what keys can you press if you're stuck in an infinite loop?
[67:46] Command C. - Yes, ooh, mm, something very similar to Command C.
[67:54] - Control C. - Yes.
[68:01] - Control C. Yes.
[68:03] What up, pseudo? And all right.
[68:10] What is the difference between break and continue? Let's see.
[68:17] Uh, break will do it when the loop is done and continue will continue to do the loop no matter what.
[68:31] - Very, very close. So break makes the loop be done.
[68:43] - Break means stop looping here and move on with whatever is next in your life.
[68:48] Continue, go to the top of the loop. - Oh, yeah, yeah, yeah, okay.
[68:56] - It doesn't necessarily mean, it's not just keep looping, it's a very specific thing.
[69:00] Go to the top. - Yeah.
[69:04] And thank you. I'm gonna see if I can say your name close to right.
[69:10] Fuck you, I hope. Thank you for saying that because I think a lot of it is,
[69:16] this is a big reason why people don't go into coding because especially if, like, being newer to it,
[69:24] yes, I'm figuring it out from the book and I'm following along with the book,
[69:30] but it's also very difficult because I'm like, uh, I don't even know where to start.
[69:36] And that's why, again, I love having Laura on because then she, like, gives me time to try it
[69:43] and then it's like, Jen's really stuck. Okay, let's try to redirect.
[69:48] All right, what is the difference between range 10, range zero comma space 10,
[69:58] and range zero comma space 10 comma space one in for loop? Honestly, I don't think we went over this.
[70:06] - I don't think we did. - But something tells me it has something to do
[70:13] with how many loops it goes through. - Yes.
[70:19] So let's use the technique that we just learned. So range is a function.
[70:23] We can tell it's a function 'cause it takes a function.
[70:26] We can tell it's a function 'cause it takes a function.
[70:28] So range is a function. So range is a function.
[70:31] We can tell it's a function 'cause it takes an input 'cause it says range parentheses 10.
[70:36] That means that that is a function and we're giving it the argument 10.
[70:41] So that means that if we type the function range into your IDE and then we hover over it,
[70:46] the IDE will tell us what it does with the arguments that we pass it.
[70:56] So like just hover, don't click. There we go.
[71:00] - Range stop. So that's the one number.
[71:09] Range object range is start stop or start stop step. - Mm-hmm.
[71:17] So there are optional arguments that we can pass to this range function.
[71:23] If we pass it just one argument, that's gonna be the number that makes it stop.
[71:29] If we pass it two numbers separated by a comma, it'll start at the first number
[71:35] and it'll stop at the second number. If we pass it three arguments,
[71:41] it'll start at the first number, stop at the second number,
[71:44] and the third number will be how much it'll increment by. So let's do one.
[71:53] - Okay. - Let's actually use this function.
[71:56] - Okay. - So let's print.
[72:02] - Can I do it on the same in this or you want me to do a new file?
[72:07] - Let's do a new file. Something I think we should work on next time
[72:13] is figuring out how to execute just a selection. And yeah.
[72:26] Oh yeah, pseudo. Yeah, it's the kind of thing
[72:29] where like when you use something forever, you don't think of it necessarily as a function.
[72:35] It's just, it's the thing. And at least that happens for me anyway.
[72:39] But it is totally a function 'cause we're passing it arguments.
[72:45] - Okay. All right.
[72:51] And as a total- - Jen, do you wanna put up the comment
[72:53] that I was just responding to? 'Cause otherwise this is gonna make no sense in the-
[72:57] - Yes, yes, thank you. Thank you.
[72:59] And as a heads up y'all, we have like 15 minutes left.
[73:08] So I think we have enough time to do the range, which apparently we're not gonna get to chapter three today,
[73:14] which is okay. You know, we're getting there.
[73:17] We're getting there. If you're interested in following along
[73:22] with our journey every Monday, please hit that follow button.
[73:25] And normally as a heads up, I totally forgot about it today.
[73:29] We also stream on Laura's stream. And today I forgot to, sorry, Laura.
[73:34] - Oh, that's okay. - I totally spaced it until like right this second.
[73:38] - No worries. - So that way she also has an audience
[73:44] that can learn a lot from Laura. That's why I really like learn with Laura.
[73:49] (laughs) Great term for Mondays.
[73:52] All right. - All right.
[73:55] - So. - So let's print.
[73:58] Let's use that 10 as an argument to print, to range, sorry.
[74:08] - There we go. So would I do range instead of print
[74:16] or I would just do print 10? - We're gonna print the range.
[74:19] So print is also a function. So we need to give it range as an argument.
[74:26] - Hold on. - Cool.
[74:38] Nope. What do we need to do when we're using functions?
[74:45] Yeah. It goes in the parentheses, exactly.
[74:48] Okay. - Yay.
[74:53] - Let's do it. - And run it?
[74:57] - Sure. Oh, sorry.
[75:02] Okay. So, right, because that's what we just,
[75:05] literally just passed it. Okay.
[75:08] So let's make. Let's make a list.
[75:15] Oh, you know what? We should really be doing this like in a loop.
[75:23] Okay. So we have, have we done four loops?
[75:30] - We. - Wait a minute.
[75:32] Did we even get as far as the quiz? I feel like we didn't because.
[75:35] - I wonder if we didn't. - I don't know 'cause we're, yeah, yeah, yeah, yeah.
[75:40] 'Cause I was like, how, what, how? I would never have said, let's just skip range.
[75:44] And then I was, I was like, was struggling here because I was trying to do range without doing a for loop.
[75:50] And then I was like, wait, why would we be doing this without a for loop?
[75:53] Yeah, we never got, we never got this far. - Oh, wow.
[75:56] And we will start here next time. Where are we starting?
[76:04] - We did importing modules. So we can go down a bit.
[76:09] Start stopping and stepping. So I don't know why we would have imported models without,
[76:13] I mean, knowing me, I probably skipped over it and not realizing I skipped over it.
[76:18] - Maybe we were just scrolling too fast. - All right, so we will start here next week.
[76:23] - No, wait, it still says. Okay, yeah.
[76:28] So we should, we should start with the, with the starting, stopping and ending arguments.
[76:33] 'Cause that is the one that we did. This one here, an equivalent while loop, I think.
[76:38] Oh no, no, no. 'Cause they're for loops above.
[76:41] Go up. - You are part of.
[76:50] - We definitely talked about truthy and falsy. I think that's where we left off was truthy and falsy.
[76:56] So scroll down a little bit. Keep going, keep going.
[77:00] We did this. 'Cause I remember you saying you liked truthy and falsy.
[77:03] - Oh yeah, and then we did this. - Right, that's where we need to pick up next time.
[77:08] Let's start with truthy and falsy just so that way we can do a recap next time.
[77:12] Yay. So.
[77:16] - Actually, did you say earlier that you wanted next time to be about like,
[77:19] was it making Incudex or something about? - I'm gonna use it as the review.
[77:26] - Okay. - So that way we can go through the review fast,
[77:29] faster and learn from it. So I'll upload those.
[77:32] But is it? No.
[77:37] What are comments in Python? - That was it, that was it.
[77:40] - Was it? Okay.
[77:42] Give me the. Yeah.
[77:46] I see. Why do you not like it?
[77:55] - Wait, is that not it? Oh, you know what?
[77:58] I think it's hashes. Is it hash?
[77:59] Try hash. - Oh, okay.
[78:03] There we go. - I think it might just be, is it two hashes?
[78:05] I think a single hash will work. - Yeah.
[78:09] - That's the one. I've been writing, I've been learning Go
[78:11] and it is slash slashing Ingo. - All right.
[78:15] So we will start with range next time with Troopsy and Falsy just to figure it out.
[78:24] And then we'll save this one. I don't know why you're not saving the entire,
[78:28] like everything, but you know, that's fine. And then, so we got that done and we got to do what I,
[78:38] oh, okay. And said, this is kind of how I've been remembering it.
[78:44] - Mm-hmm, mm-hmm. - Status and changes.
[78:50] I want to do, and I want to do them all. So I'll do bit, period.
[79:02] - Mm-hmm. - And then.
[79:04] - So what that period means is everything in this directory. - Right, so if I only wanted to change spam,
[79:12] I wouldn't change, I would type spam.py instead of period. - Sure, yeah.
[79:21] That dot though, like referring to what's going on in this directory is not just a get thing.
[79:26] - Oh. - Like when you do code space dot.
[79:30] - Mm-hmm. - You're saying open in code, everything in this directory.
[79:35] It's the same dot. - Oh.
[79:37] - It means the same thing. - Okay, okay.
[79:40] - That's where it comes from. At least it helps me to remember things
[79:43] when I know like what they mean, instead of just like, this is the dance you do
[79:48] to make this thing happen. - And then, so get, push or get commit?
[79:56] - You have to commit before you can push. - Commit bash m.
[80:04] - You will need quotation marks around the string that you're adding.
[80:19] - And then, oh.
[80:25] - So that's about configuring how get works on your machine. It's not a problem.
[80:45] - Yeah. You can suppress this message by setting them explicitly.
[80:51] - Mm-hmm. - So.
[80:55] User.email would, I would just change this part, right? Whatever, I'm not gonna do it right now.
[81:10] - I would recommend not doing it right now. - I'll figure it out next time.
[81:14] So we'll do get, wait. Commit, we gotta do get push.
[81:22] - Right. And does that one have a comment too?
[81:24] - You, no, only commit messages. Like, in fact, it's such a commit thing to have a message
[81:35] that I didn't even just say the commit, I said commit message.
[81:38] So like tied together in the memory. - One minute, it added them.
[81:49] - Mm-hmm. So, and then just to double check,
[81:53] like knowledge fact check myself, if I was to have a branch,
[82:00] but if I was like in somebody else's repo, I would have created my own branch,
[82:11] then created a pull request to submit it. - Mm-hmm, exactly.
[82:16] - But everything else would have been the same. - Yeah.
[82:20] - Like, okay. Okay, okay.
[82:23] We're getting there. We're getting there.
[82:25] - Totally are. - Oy, oy.
[82:29] My head is a little mushy, but that is okay. Later today, I get to do some JavaScript
[82:37] and I'll probably live stream for that at some point today. I'm not sure.
[82:43] I just know that I need to do some type of 100 days of code and so I'm going to do that
[82:52] because a lot of my other streams are based on JavaScript. And at the moment, I've been keeping them pretty separate.
[83:02] Like they make enough sense separately, but we'll find out if I get really stuck later on.
[83:07] - Sure. - But, and then also setting up OBS.
[83:12] So exciting extra streams this week. That will just be random.
[83:19] Tomorrow, everyone, we will be doing Svelte versus React app an hour early
[83:28] because of our guests could only get on an hour early with Brittany Postma and Anthony,
[83:35] who I just told him his new last name is AJCWebDev. 'Cause I always forget.
[83:43] - You know, I would get 1080p if I had extra money. So if you want to subscribe and give money,
[83:53] that's when I would. 'Cause StreamYard, you have to have
[83:57] like the even more extensive package to get 1080p. And unfortunately that's not something
[84:03] in the price range right now. Hopefully I get a job soon.
[84:07] I am applying places. I am interviewing places, but we will see.
[84:11] So if you also know anyone looking for DevRels, that is what I do.
[84:16] And yeah, that is when. So, okay.
[84:22] There, pseudo answered the question themselves. StreamYard or StreamYard, OBS instead of StreamYard.
[84:31] See if I can talk. Well, even better.
[84:33] Then we will be hopefully doing that next week. So I'll get 1080p sometime this week.
[84:38] So if it's not the normal time, you should come check if I'm actually trying to set up OBS.
[84:45] That is good. And thank you, thank you, thank you.
[84:49] And thank you everyone for joining today. I look forward to seeing you tomorrow
[84:53] and Laura will be back next week. - Yes.
[84:57] - And she's feeling better than last week in case anybody was curious.
[85:00] I did ask because you're also not coughing as much. So I am very grateful you're feeling better.
[85:06] - So am I, thank you. And thank you for teaching us all the things.
[85:10] Bye everyone. 
