---
showLink: "https://www.youtube.com/watch?v=h8A80AYsRQQ"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "automate-the-boring-stuff-with-python-with-laura"
title: "Automate the Boring Stuff with Python with Laura"
publishDate: "2023-03-10"
coverImage: "https://i.ytimg.com/vi/h8A80AYsRQQ/maxresdefault.jpg"
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

[00:00] >> Hello, hello, beautiful humans. Welcome back to a long-awaited,
[00:06] Jen has a streamed in forever, teach Gen Tech episode about Python.
[00:12] Hello, Laura. >> Hello, Jen.
[00:15] >> I'm excited for Python. We haven't done this in- >> Yes.
[00:19] >> Oh, gosh. I think it's been almost a month. It's almost been a month, which is crazy.
[00:25] For those who don't know, and this is a big reason why it's been so long,
[00:29] is I started a new job, yay. I work at a database infrastructure company called Ivan.
[00:40] A few days after I started, we had to fly to Finland for our DevRel off-site.
[00:48] In the process of that, I got COVID and pneumonia and was a really hot mess,
[00:54] and finally better. I was like, "Oh, I totally got to stop streaming."
[01:00] For some reason, that's what I thought. They're like, "No, Jen, we want you to stream.
[01:04] Keep doing what you're doing." I'm like, "Oh, okay."
[01:09] The biggest news on all of that is we will continue streaming. It's just going to be a different time.
[01:16] It's going to be a little later in the day because Ivan is based in Finland and I need
[01:23] more time in the morning to work with the humans at the company. What updates do you have for us, Laura?
[01:32] Anything you want to share? >> Well, I'm going to start using
[01:43] NeoVim as my primary editor for a while. I am learning all kinds of things.
[01:49] I've already been using Vim key bindings for a while, and using Vim in my terminal for some kinds of stuff like
[01:57] editing my Z-Shell files, like any dot files or whatever.
[02:03] Yeah, I tried to do some things in VS Code and they just weren't working in VS Code,
[02:10] but they were working in my terminal, which meant that it's not something that's wrong with the program,
[02:15] but it's something that's wrong in VS Code. I was like, "You know what?
[02:19] I'm going to do Vim," and then I was like, "If I'm going to do Vim,
[02:23] I need some plugins." Then that sucked,
[02:28] and then it turned out that there's this fork of Vim called NeoVim that has a much better plugin ecosystem.
[02:34] I was like, "All right, I guess I'll use that." Now I'm down this rabbit hole series.
[02:41] It's getting interesting. >> Yeah, and I am going to have a.
[02:48] You know how if you want to open up some files with VS Code, then in your terminal, you can type code space dot code,
[03:00] open everything in this directory up in code. You can do that with Vim and you can do it with NeoVim,
[03:06] and the acronym nvim is what you use. You would type like nvim, whatever.
[03:15] I am going to start, I think maybe a blog series or maybe some recordings,
[03:24] and it's going to be called Becoming Invincible. >> Oh, I love that.
[03:30] I love that. >> He's here with me, so I'm excited.
[03:34] >> You and Vim, you have fun with that. That's what I have to say about,
[03:40] you have fun with that. I mean, eventually, I feel like I'll probably
[03:45] ask you more questions about it, but I am that person, just so everyone knows.
[03:51] I am that person that is like, I got stuck in Vim somehow,
[03:55] I'm just going to close my terminal and restart because I don't.
[03:59] >> Haven't we all, honestly. >> So, yeah.
[04:03] I feel like it's something that is definitely going to be something to go into in the long-term.
[04:13] It would be good to know. Yet, on Monday, because y'all,
[04:19] we will still have MISC Monday with the two of us. I have some things to show Laura and everyone about my,
[04:27] I'm going to be starting a new data infrastructure series, and having guests on about that.
[04:35] Next week is my first guest in that series, and it's Lucia from Confluent,
[04:43] and we are talking about Kafka. Kafka?
[04:46] Kafka. I don't know.
[04:47] Kafka, Kafka? >> I would be inclined to say Kafka,
[04:51] but I have absolutely no idea if that's correct. >> Yeah, I've heard both.
[04:56] I feel like I've heard both. I don't know, I could be just making it up.
[04:59] I will ask her, but yes. So back to Python, which I'm slightly dreading
[05:08] because this week's chapter just none of it made sense. And yeah, it's a lot of terminology that I've used.
[05:24] I've used in JavaScript, like I can visualize a lot of it, but I'm like, it's still not 100 percent clicking.
[05:33] So let's get into, I will post chapter 3 of "Animate the Boring Stuff" and share my screen
[05:48] because that would be helpful. All right.
[05:52] Oh, and because everyone, and this is something that's from another conversation, but I do want to share,
[05:59] we eventually will be using OBS. This has been a goal for many months.
[06:06] One of my new colleagues is going to help me go through the different scenes I need to create and kind of,
[06:18] I feel like, I almost feel like I'm being a baby about it because I'm like, this is just taking so much time
[06:24] that I keep avoiding it. Like I understand it, but I'm like,
[06:27] I'm just not computing on it. So I'm very excited for that.
[06:33] We're not going to stream it. It is going to be done behind the scenes,
[06:35] but I'm just excited to be able to tell you that we're going to have OBS at some point.
[06:41] So OBS is like the vim of streaming. Ooh, I think that is a good way of saying it.
[06:51] I will grab, just so that way people see it in our chat, that is OBS, and then also I'll be using a tool called Ping
[07:09] that is like StreamYard for OBS. Someday I'll probably explain it.
[07:18] For now, I just need to actually get it set up. That is something that along all of this live learning,
[07:26] something that I've learned about live learning, sometimes I need to learn something offline.
[07:32] Sure. Which I didn't expect.
[07:35] I was like, sometimes I just need no distractions to learn it.
[07:40] Yep. And yeah, well, functions is not one of them.
[07:46] OK. So we are on chapter 3 of Automate the Boring Stuff.
[07:54] And previously, if I go back-- let's actually go back to the summary of the last one,
[08:03] just so that way everyone can scroll. So we're scrolling to the summary.
[08:10] I probably could have done Control-Find, and that would have probably made this a lot better.
[08:15] But you know what? We are just going to keep scrolling to the bottom.
[08:21] And I will think about this in a second. So in Vim, if you press capital G, it takes you to the bottom.
[08:27] Oh. I'm just going to be making Vim jokes all the time now.
[08:31] I feel like you are, but I'm OK with it because it's like-- oh, and for those who have been following
[08:40] Laura's and my Vim streams-- there we go-- for a while, on the last Misc Monday,
[08:49] we were talking about COVID and masks and stuff like that. And I feel like it is kind of funny.
[08:58] Not funny-funny, but I wouldn't say ironic. It's not the definition of ironic.
[09:03] But it's interesting that I ended up getting COVID. But I think I got it from planes.
[09:09] And so one thing that I need to remember is to ask Laura to send me the COVID mask.
[09:16] Because I feel like, personally, in my little progression of thinking about all of this, that I will probably not wear
[09:25] masks in the airports and conferences. But on the actual airplane, I am masking up.
[09:31] I'm not going to eat anything. I am literally just going to mask
[09:34] because it circulates air, and people are really, really close to you.
[09:41] Are you interested in hearing some thoughts about that? Of course not.
[09:50] OK. So when the plane is actually flying,
[09:55] that's the safest part of your journey because they have the filtration going.
[10:01] And so the aerosols don't-- you can sort of think of it like the aerosols
[10:07] are teensy-teensy little bubbles, right? And they can't just hang around in front of your face
[10:13] for you to breathe them in with the filtration going, especially if you have the AC that gets blowing, whatever.
[10:22] So because there's so much air moving and because the filtration system is filtering the air,
[10:28] that's the safest part. The least safe part is the part where you get on the plane
[10:32] and the filtration system isn't running yet. So people have done it with CO2 monitors,
[10:38] and so the time between when you get on the plane and when you've been in the air for a while,
[10:44] that's the least safe time. Cool.
[10:48] I plan on wearing it during that time. Basically, I'm going to go hang out,
[10:53] and then when they're like, hey, come board, I'm going to be like, mask, is what the plan was.
[10:59] I say that because I am asthmatic, and hanging out, waiting for COVID
[11:08] to go away in another country without all of my asthmic gear is one of the worst experiences I've ever had.
[11:16] It also probably went to pneumonia and what caused it to go to pneumonia.
[11:22] And advice for everybody, please go research a country and what you do for medication and doctor visits
[11:33] and things like that in case anything happens. I say that because I should have.
[11:37] So it's all a lesson learned and progress, but it is also something that I have
[11:43] found very kind of my new company because I've seen it where people get really mad,
[11:51] like if you get sick, and they make you work anyway. And this company was like, bro, just chill out.
[11:59] Get better. Take care of you.
[12:00] It's the way to be. And I thought it was really cool.
[12:04] And in case anybody ever questions it, I do not sound like the people that actually talk to me.
[12:10] I paraphrase horribly in a really fun way. So please know that my company did not actually say bro.
[12:18] I would giggle if any of the Finnish humans actually said that to me because they are very proper, at least
[12:25] the ones that I've met so far. But anyway, I know, I know, I'm rambling.
[12:30] It's hard not to because we haven't had a MISC Monday in for so long.
[12:35] Back to Python, back to Python. Focus on the Python.
[12:42] So this is the summary of the last chapter, which we did with Jay Miller.
[12:48] And the summary is, by using expressions that evaluate true or false, also called conditions,
[12:57] you can write programs that make decisions on what code to execute and what code to skip.
[13:03] You can also execute code over and over again in a loop while certain condition evaluates to true.
[13:11] The break and continue statements are useful if you need to exit a loop
[13:17] or jump back to the loop start. These flow control statements will let you write
[13:23] more intelligent programs. You can also use another type of flow control
[13:27] by writing your own functions, which will be the topic of the next chapter.
[13:32] And as a reminder for everyone, because I feel like I have to call this out,
[13:38] but I'm also very self-conscious, I am horribly dyslexic.
[13:42] So trying to read out loud should be hard for me. And I appreciate that there has never
[13:48] been shame or meanness from Laura. And I appreciate that.
[13:54] So thank you. And all right, so that is a summary for last time,
[14:01] last stream with Jay, which was super fun. He had us writing a lot of creative projects
[14:09] about eyeglasses and being a glasses store. And it was an extra long stream that was so fun.
[14:16] So now we are on to chapter 3, which is functions. And this is not my favorite, which happens a lot,
[14:30] I feel like, when I end up talking to Laura of this isn't my favorite.
[14:35] And then I like it once I understand it. It's a total thing, right?
[14:40] I mean, not like a me-specific thing, but it's a human thing to feel animosity a bit towards stuff
[14:50] that you've tried to understand and you don't understand if there's a little bit of a, well,
[14:55] fuck you very much then feeling, like the brain is doing that. But then if you can get past that and be like, no, it's OK.
[15:05] We are not under threat by the fact that we don't know this thing because it's your amygdala.
[15:10] It's like your stress response because we've got these brains that evolved a very long time
[15:16] before functions in Python, right? And so if we feel like we don't know what's going on,
[15:24] then maybe it's like our brain is like, if we don't know what's going on,
[15:27] then maybe there's actually a lion behind that tree and a bug guy.
[15:31] And note for this, for everyone that might be joining for the first time or need a quick reminder,
[15:38] Laura used to be a math professor. So it's really amazing in the fact
[15:44] that it helps that she has a teaching background. But then also something that I've
[15:53] learned while working with Laura is my own way of learning things and how to work through them.
[15:59] Because y'all, I passed high school, which is around the age of 18.
[16:07] So all of my grades going up, a GPA, like a good GPA, grade point average, is a 4.0.
[16:16] Or sometimes you can get higher with extra credit. So I had a GPA when I graduated of a 1.6.
[16:26] I passed with D's. And I still got a degree, got my high school diploma.
[16:33] I say all of that because a lot of it, I didn't know how to study or how to work through a lot of it.
[16:40] And also, I didn't realize I was ADHD or dyslexic or any of that and had a lot of trauma
[16:47] going on at home, which all goes into learning. So back story on that.
[16:54] But thank you, yes, because I would love to just close this book and forget about learning Python.
[17:00] But I'm really excited to learn Python. And Laura and Jay and so many others that we adore
[17:06] keep me going, so I don't quit learning this. And y'all don't quit learning this.
[17:10] So functions. Yeah, OK, so have you--
[17:16] because I know you have more experience in JavaScript. Have you worked with functions in JavaScript?
[17:23] Yes, in the fact-- and this is good knowledge for everybody too, of I have worked with a ton of JavaScript, TypeScript,
[17:34] a lot of CSS, like Tailwind. I've worked with a lot of this.
[17:40] Figuring out how to get it to do what I want it to do doesn't mean I know what it was called.
[17:46] Sure. So I've worked with functions.
[17:48] I know they exist. But if I were to look at some code,
[17:52] I wouldn't be able to tell you that is a function. OK, yeah, OK, cool.
[18:04] OK, so how do you-- because this is your learning journey. How do you want to start today?
[18:12] I would say, first off, by-- I'm going to scroll down a little bit.
[18:18] Yes, in the last chapter, we totally went through print, input, and len.
[18:23] And that was helpful. We went through all of that.
[18:27] And then it says, a function is a mini program within a function.
[18:33] And I'm like, program, yes. A function is a mini program within a program.
[18:39] And I'm like, OK. So don't worry about that.
[18:47] We'll revisit that. OK.
[18:51] Do we have an example here of a function if we scroll down? This one's a function.
[18:58] It's too small. I feel like it's too small to understand what's
[19:02] going on for understanding what a function is, potentially. OK, I'm going to see when we go into def statements.
[19:14] Yeah, let's start here. OK, so let's type this in.
[19:21] Let's do a Jupyter Notebook. OK, what is-- and we were talking about this
[19:25] a little beforehand, so I would love to hear your definitions of, I'm in VS Code.
[19:31] I'm going to new file. And then we have a Python file in Jupyter Notebook.
[19:37] Jay told us a little bit about his views on this, too. But I'm curious what your views are
[19:41] and why we might use one over the other. So in production, I think that this is maybe slightly changing.
[19:56] But that's a very, very new thing. So we're just going to say, usually, in production,
[20:01] you would just be running a Python file. A notebook is like--
[20:08] let's get one open. Oh, we could even do-- well, I guess
[20:18] we could do both so that you could see the difference. Because I can describe the difference,
[20:22] but that's not as good as seeing the difference. All right, I got a notebook open.
[20:27] And I will do a new file. And we're going to do a new Python file.
[20:32] All right. OK.
[20:35] We're going to close this just so we have more area. I can switch back and forth up here.
[20:41] In fact, you can show both of them. Oh, yes.
[20:47] Is that one? No.
[20:51] Yeah, if you-- yeah, split right and then close the first one. The one on the left.
[20:59] Yeah, there you go. OK, so grab that code.
[21:04] And I think it's great that you can't actually just copy and paste it, because then you can--
[21:11] You could copy and paste it. Because then we can talk about it.
[21:21] There we go. OK.
[21:23] Oh, I got to move my book, because I'm still figuring out my whole desk set up when I actually
[21:27] need to type. Oh, it already indented.
[21:41] Print. Print.
[21:42] Print. [21:43], print.
[21:43], print. [21:44], print.
[21:44] the name. The name.
[21:55] The name. The name.
[21:57] The name. All right, it has been typed.
[22:28] OK, so all right, let's work just in the notebook at the moment.
[22:40] And once you're feeling good about this block, then we'll see the difference between-- actually,
[22:46] we need to have more than one block to see the difference between a notebook and just a Python
[22:52] file. Oh, perfect.
[22:54] OK. So great, so we will revisit.
[22:57] We'll come back to the Python file itself in a bit. OK, so that def, what do you think that stands for?
[23:07] It's defining hello? We are defining a function, and that function is called hello.
[23:14] And that name that's in parentheses, what are your feels about your sense of what that is?
[23:22] A variable. A variable.
[23:27] Sure, yeah. And when we pass a variable to a function,
[23:34] it's called a parameter or an argument. I was going to say an argument.
[23:39] I don't remember parameter, but I remember argument. Sure.
[23:43] Cool. Yay.
[23:44] OK. And so we're saying, hey, we're going to make this function.
[23:49] It's going to be called hello. And what we're going to give to hello as an input
[23:55] is going to be this thing called name. OK.
[23:59] And then on the next line down, we're going to-- the function is going to print hello and then add--
[24:08] it's going to append the name at the end of that string. So it's going to print hello and then the name as well, right?
[24:16] Yeah. So let's run this.
[24:21] I'm doing-- so for those who may be like, Jen, what are you doing?
[24:29] I am-- so up here, if I go just really briefly trying to put two and two together, basically the first function
[24:38] is saying it did define hello and then print these three. So it gave it three different options.
[24:49] And so I printed it three times because it had three hellos. And what I'm trying to see is just like, if I do this,
[25:02] is it going to do-- instead of just hello, Bob and Alice, is it going to do hello, Bob, Alice, Laura, and Jay?
[25:11] OK, yeah. So-- and--
[25:16] CB-- CBid-- What up, Chrissy?
[25:19] Oh. Hello.
[25:22] At least I hope so because if there's somebody else with this name, I'm
[25:26] going to be really confused because she's the one who posts about badass women in tech
[25:30] and she is one as well. And she does a lot of really good content.
[25:35] At least Chrissy does. If CB-- CBid2, if you're not Chrissy,
[25:40] then I'm really sorry that I'm not putting two and two together.
[25:42] You can tell me I'm being mean. It's fine.
[25:46] But anyway, so yeah. Right, OK.
[25:55] So and then let's just run this. Let me make this bigger.
[25:59] I just realized that I hate it when they're really small for me and it doesn't always look small for streamers.
[26:07] Right, yeah. Oh, I thought I already installed it.
[26:11] OK, well, let's see if we can install this really quick. And yay, it is Chrissy.
[26:17] Yay, hello. Let's see.
[26:20] I'm going to, while this is installing, distract myself with some Twitter and go.
[26:27] I know-- oh, go ahead. I posted on Mastodon and tagged you.
[26:37] Oh, yay. This is Chrissy's information to see all the dope stuff
[26:46] she's doing. Nice.
[26:50] I just wanted to put that really quick. Yay, and it printed them all.
[26:56] So out of curiosity, if I do this line again of the same thing, or maybe I'll put "bye" just so that way.
[27:08] Bye, no, I need comma, plus name. Now what happens?
[27:19] Oh, that's kind of cool. I don't quite fully understand it, but that's cool.
[27:25] Which part? The fact that it didn't group all of the hellos
[27:36] and then all of the goodbyes. OK, OK, OK.
[27:42] So how to think about this. So you called first.
[27:51] You called "hello," and you gave it the string "Alice." And so what it's going to do is it's going to say, OK,
[27:59] I take "Alice," and what I do first is I print "Hello, Alice." And then the next thing that I do, the function "hello,"
[28:11] the next thing that I do is I print "Bye, Alice." So I ran through my whole function, and then I'm done.
[28:22] So now I can go to the next line down, which is "Hello, Bob." And so what do I do with Bob?
[28:31] I say "Hello, Bob," and then I say "Bye, Bob." Now I'm done with that line.
[28:36] Now I can go to the next one. I print "Hello, Laura," "Bye, Laura."
[28:42] So if you wanted it to group all the hellos and the byes, you would need to have two functions.
[28:53] You could have a "hello" function and a "bye" function. It does go through that later on a bit,
[28:58] but something that I think might be something that other newbies might relate to is the fact --
[29:06] so getting -- I'm going to just say this box functioning or working -- I won't even say function yet --
[29:15] being able to do whatever that needs to do, I could do that. Like, I'm like, "Okay, cool. Like, this totally makes sense.
[29:22] I'll play around with it until I -- enough until I get it to do what I want it to do."
[29:26] Yet if somebody asked me if I knew what function was, "Nah," because I didn't learn it with what it was,
[29:38] I could just make it work. -Sure. Yeah. Okay.
[29:42] So can we -- VS Code has, like, code spaces, right?
[29:56] Because I was just thinking, like, it would be great if I could type in this thing right now.
[30:00] -Oh, yeah. Like, I can live-share with you. -Okay. -Yeah.
[30:08] I'm going to go off-screen for a second because -- oh, wrong one. This one.
[30:14] Because I don't need everybody to join us because that could be kind of awkward
[30:18] if there's a ton of us in the same area. So it is signing in right now.
[30:24] And then I will send you the link, Laura. -All righty.
[30:28] -Maybe. Maybe I will. We'll find out.
[30:35] Oh, I didn't click the thing above it. That would help.
[30:49] Yay. And private chat. What?
[31:03] Okay. I haven't actually done this before.
[31:24] -Ah. You might have to install. -Install the extension, which is pretty cool.
[31:33] One of the DevRels on my team, Sebby, just made an extension for the product, VS Code extension.
[31:45] And I just thought that was so cool. I was like, these are, like, you can do so much with open source.
[31:51] -So, let's see. I clicked the link,
[31:54] and it asked me if I wanted to open in VS Code. And I said, "Yes."
[32:00] But it just -- Oh, there it is. -Can you see the things and stuff?
[32:17] -Maybe. It's thinking. Joining collaborative session, it says.
[32:21] -Oh, I can see you now. -Ooh.
[32:24] -Laura is on Twitter but mostly Mastodon. Like, Laura, do you even reply on your Twitter?
[32:32] -Um, I check it once in a while, but I mostly am not. I'm trying to see.
[32:43] -I've got your website. You concentrate on that.
[32:46] Your website has all your links, right? -It does. Yep.
[32:50] -All right. There we go.
[32:54] Good call-out, Chrissy. I appreciate that.
[33:01] -I have to sign in. -Oh, I know.
[33:07] -Doo-doo. -I love how -- And, Chrissy,
[33:11] I feel like you need to come on the show sometime, too. Chrissy has talked about, like, she does --
[33:19] I feel like it's really good -- I don't know if it's marketing is the right way of saying it,
[33:23] but, like, while she's, like, promoting other people, she mentions, like, what she's working on, too.
[33:28] So people, like, if I repost something that she posted about me,
[33:33] people can see how to get in contact with her. I was like, "Dude, that's genius."
[33:37] -Nice. -I wish I thought of that back in the day.
[33:41] -Okay, so you can see me, can you? Did you say? -Yeah, yeah.
[33:45] -Oh, can you re-share your screen so I can see what you're seeing?
[33:49] -Yes. Give me a second. Na-na-na-na-na-na.
[33:54] It's this one. -'Cause I don't see, like, under live workspace,
[34:02] live share workspace, I don't actually see any files. -Oh.
[34:07] Well, it says you're not currently editing your -- the documents,
[34:11] but you're in the participation. Weird. -Okay.
[34:16] -Can you click me to say "follow"? -I don't see anything like that.
[34:21] -Oh. Oh, nope, I don't want to e-mail you like that.
[34:29] -Live share workspace, yes. It's open.
[34:32] Oh, okay. I have to trust this workspace.
[34:39] -Ah. -Maybe. Maybe that's going to give me what I need.
[34:45] -Uh... Sure.
[34:52] Okay. Why is this not -- Okay.
[34:59] Okay, one more time. -See, it will say that you joined.
[35:10] -Uh-huh. Huh.
[35:16] I don't know. 'Cause, yeah, I see nothing.
[35:25] Okay, well, we'll fix this out. Oh, I've been removed.
[35:29] -Yeah, I tried to kick you out just to see if you could rejoin and -- -Yeah.
[35:33] -'Cause it had you in multiple times. Maybe that will be it.
[35:36] Yay! Chrissy followed you on -- -Okay, I'm joining.
[35:39] -The LinkedIn. The LinkedIn and stuff.
[35:42] Ooh, thank you. No.
[35:49] Okay, well, we should figure that out sometime. -We'll do it another time.
[35:54] That is fine. We also -- -Yeah.
[35:57] -Oh, yay! And HashNode.
[36:02] -Yay. Um...
[36:05] What was I going to say? I have no idea.
[36:09] Anyway, so what I was going to do was say, like, I think that part of what's hard to understand maybe about --
[36:19] not that it's hard to understand about functions, but that sometimes when we're teaching,
[36:25] we try to, like, break things down into, like, the smallest unit possible.
[36:29] -Mm-hmm. -But sometimes, like, if you're seeing it out of context,
[36:33] it doesn't totally make sense, like, what it's doing. So, like, when it says a function is, like,
[36:40] a mini-program within a program, all that this program is right now is one function.
[36:46] And so it's hard to see, like, the mini-program-ness because it's not existing in a larger program.
[36:56] -That's really starting to make sense. -If that makes sense.
[36:59] Okay, yeah. So let's put in another block into our Jupyter Notebook.
[37:12] I'm only trying to click on things like that's a real thing. Okay, and let's put it above the --
[37:18] I think you can just drag it maybe. -Yeah, I think so.
[37:23] Let's see. Drag.
[37:25] Go above. Go all the way up here.
[37:27] Yay! -Yay!
[37:29] -So all the way to the top. Yeah, okay, cool.
[37:32] So, oh. Okay, I officially think that we'll be better off
[37:39] in the Python file for this because I think it'll make it a little bit clearer
[37:44] how the function fits within the larger program if they're not visually separate blocks.
[37:53] -All right. -So let's pop over.
[37:55] Just copy and paste that code. -Copy, paste.
[38:03] I'll just close this for now. No, I just actually just --
[38:09] I don't want you to close, close. I just -- whatever.
[38:11] It's good. -Yeah, you can just make it all the way smaller, whatever.
[38:16] Okay. So, right.
[38:21] So now above line 1, let's get some more -- let's get some more lines above line 1.
[38:31] Okay. So now let's --
[38:38] let's print something like "Welcome to Teach Gen Tech." Okay, cool.
[39:06] And then -- you know what?
[39:16] Just for the sake of -- well, no, never mind, never mind. Teach one thing at a time, Laura, one thing.
[39:21] Okay, so on line 3, let's print -- what's your name?
[39:36] Or no, let's make a new function. So let's type "def," space, and, like, "get name."
[39:51] We can make this function be called "get name." And then a colon after the closed parens.
[40:07] And then get another new line. And so in some languages,
[40:18] you have to put semicolons at the ends of all of your lines so that the computer can understand, like,
[40:26] where new lines happen and so on, and, like, how things relate to each other.
[40:32] And you have to, like, put braces inside of things and so on. So Python, you don't have to do the semicolons,
[40:39] and you don't have to do the braces most of the time, because it relies upon whitespace.
[40:47] So you do have to do the indentation. Okay.
[40:55] That matters. And it'll get mad if you have indentations that don't match,
[41:00] but we can get to that later. Cool.
[41:04] So in "get name," let's put -- we're going to use a function called "input,"
[41:13] which we have used before. Yes.
[41:17] And we're going to give it a -- let's see.
[41:24] We are going to assign input to -- let's just use "name."
[41:34] So that would be using "name" as an argument to input. What we want instead is to put "name" equals "input."
[41:44] Oh, okay. "Name" equals "input."
[41:53] And "input" does need the parens on the end. Okay.
[42:03] So let's comment out the "hello" -- everything from line 6 down. Let's just comment that out.
[42:17] And in case anybody wants to know a really easy way of commenting out, at least on Mac, it is "command this."
[42:29] I don't even know what this is. "Command this to comment out many lines."
[42:38] That's not a Mac thing. It's an IDE thing.
[42:44] So VS Code is what's doing that for you. But most IDEs, at least the IDEs that I've played with, have all done that.
[42:53] Nice. Yeah.
[42:55] All right. Okay.
[42:57] So let's run this program and see how we're doing so far. Not going to lie on this one.
[43:04] I don't remember how to run it. So go up to the top bar.
[43:11] Okay. Top, top, top.
[43:14] Yep. And there's one that says "run."
[43:17] Oh, yes. Okay.
[43:21] Start debugging. Let's run that.
[43:23] Run without debugging. Yeah.
[43:27] And it wants a name for this. Okay.
[43:33] So it printed, "Welcome to TeachGen Tech. Learning Python."
[43:38] Because that's what we have on our first line. And so far, that "get name" function doesn't have any output.
[43:48] Right? It literally only has an input.
[43:51] Right. Yeah.
[43:53] So it hasn't done anything yet. So what we could do is print above line four.
[43:58] We can get another line in front of line four. Print, "What's your name?"
[44:15] That's much better. I don't get why you can't use proper grammar.
[44:27] Okay. So you can.
[44:29] Hang on. Hang on.
[44:31] I'm struggle busing just like it is. There we go.
[44:33] Okay. So you can instead use.
[44:37] So before "hey" and after the quotation mark, you have a single quote.
[44:43] Yes. Make those double quotes.
[44:45] Oh. Okay.
[44:50] And now you can put an apostrophe before the "s." Yay.
[44:54] Because what was happening before was you had a single quote in front of the "hey" and then a single quote,
[45:00] because single quote and apostrophe are the same keystroke. Right?
[45:04] And so it doesn't know the difference. So it was like, okay,
[45:07] you want to start this string with "hey" and you want to end it with "what?" Because that's where you closed it.
[45:13] Make sense? Yeah.
[45:15] Yep. So single quotes do work for strings in Python,
[45:20] but if you're going to want to use apostrophes, you're going to have to use double quotes on the end.
[45:26] Or like on the two ends. Okay.
[45:30] So what does this do? It will give us a space to input our name.
[45:37] Let's run it. The lack of repo.
[45:45] Chrissy just said, don't get me started on the lack of that in repo docs.
[45:53] Oh, for commenting out like? Yeah.
[45:56] I bet. I'm guessing at least.
[45:59] Yeah, I could see that. Okay.
[46:02] We're going to hit run. We're going to be in this one.
[46:05] And now we're going to hit run. And it wants us to enter something, but it's not showing my print.
[46:16] Why are you not showing my print? Let's say.
[46:20] Okay. Comment out the name equals input line.
[46:30] And let's just run it without that and see. What we have.
[46:38] Comment out is like my favorite thing in the world. Oh, what are you doing?
[46:45] Oh, you're in your terminal. Go to output instead.
[46:56] Okay. And so it can't find.
[47:00] Oh, this is an X code thing. This is like the fun of streaming with me is like,
[47:08] it doesn't matter what computer I'm on. I like to find this kind of stuff.
[47:14] A magic. Okay.
[47:21] Ran it, but it still didn't say hello. Okay.
[47:26] So, well, we haven't called it. So that is expected.
[47:35] This is why I wish I could be typing with you right now. Okay.
[47:41] So let's, let's call the function. So below on like line six, get some more new lines.
[47:53] And, and let's call our get name function. So good name.
[48:04] And then I'm looking at what we have down here and then we're going to do. And then I don't know after that, like.
[48:18] Would I just put a comma after this one? Did you say a comma?
[48:24] Yeah. What is pinging for you that you feel like you might need a comma?
[48:32] Oh, just kidding. I thought I saw one down here.
[48:38] And then what I just say, get name is name. So, if you look at our get name function definition.
[48:47] Do we say that we're going to need any arguments? An argument means that.
[49:04] I feel like I know this backwards, but not this context. So where would we look to see if get name needs any arguments.
[49:19] In here because that's where we got good name but. So, so we forget because I agree.
[49:26] Argument always makes me think of like the word argument like in English not in coding, but I got it earlier which is the frustrating part. What do we need to say input.
[49:40] So scroll back down to the other the hello function. Okay.
[49:45] Scroll back up a little bit. Alright, so looking at line nine.
[49:49] Okay, there is an argument on line nine, where is it, or what is it rather. It has name with name is the argument.
[49:59] Inside the parentheses. Okay.
[50:02] There are no arguments inside the parentheses of get name on line three. So that would be if we're going to like try to make a function. So look at stop scrolling for a sec.
[50:16] Look at line three. Get name has no arguments.
[50:25] There we go. And we don't need the colon because we're not defining a function, we're using a function. Okay.
[50:33] Okay, so let's run this. See if we can get around the Xcode problem. Yay.
[50:43] Okay, and now we can input. Okay, great.
[50:53] Okay, so that that is that function. So far, is printing. Hey beautiful human what's your name, and then it's getting the input, but it's not doing anything with it. So we want it to return the name.
[51:14] This so the get name function has, has an input functions don't have to have an output. But we want this function to have an output, because we want it to get us to get our, our name.
[51:32] Oh. What you doing?
[51:39] I don't know. Okay. That's fair, trying to figure out if this makes sense.
[51:46] I don't know if it does, but I was going to type and see what happened. I didn't like do something like this.
[51:56] Um, what we need to do is adjust we need to add to, we need to add an output, like a notion of an output to our get name function. So we don't need what you just put in line eight, let's take that out.
[52:16] Okay. And under line five we need another new line. Oh, you know what, could you make the terminal, a bit smaller so that we can see more of the. There we go. Okay, great.
[52:33] So, put a new line after line five. Okay, and type return space name.
[52:51] Okay. So, let's, let's, um, under, or rather before get name on line eight.
[53:12] Put name equals get name. And then we'll talk about what's happening so let's run this.
[53:32] Everything's still working. And then, um, now, uncomment the the hello function, but not, not the Alice and Bob and stuff just the hello function. Okay.
[53:55] Now let's run this. Oh, are you, does it, are you auto saving.
[54:19] I keep saving it but I don't know, I'm just going to do better spacing. Oh, save again.
[54:28] And then click run. Oh, sorry, we didn't actually use it so we defined the function hello, but then we didn't actually do anything.
[54:40] It already has an output sorry nevermind don't listen to me. Yeah. Right.
[54:48] Okay, so what could be happening here so we've got. We've got the name.
[54:55] Let's go back to. Hello. Oh, you know what, comment, or nevermind don't comment out just under online nine, just write a print name, and let's just make sure that things are working the way that we think they are. And really quick.
[55:18] Thank you. We have a comment from, I don't know how I would say your username. Curious is curiousness is gold, just trying out how things work or break is a great avenue for learning. Thank you. It is embarrassing sometimes because I'm like I really want to get this in right it doesn't always click, which is frustrating.
[55:45] But, thank you know that this isn't what fuck around and find out actually means. But, but, you know, it has it has a flavor of fuck around and find out. Right. I feel like it's like a more structured version.
[56:01] It's certainly it's certainly a less physically painful version. I don't know, because there's times where I say that because learning live is like this way of.
[56:16] It can be very embarrassing and still give me like the physical feeling of anxiety. It's like pushing through that can be pretty easy because I get used to it, but on other days it's like, I'm really still struggling. So, hey, we got it. All right, printed printed the name. That's good. Okay, for the follow.
[56:48] Rob. Okay, and so we still need to call our Hello function so we defined our Hello function, and underneath that we're going to call it.
[56:59] So, let's get a new line. And we're going to unindent.
[57:10] Because we're not. This isn't going to be part of the Hello function, this is going to use the Hello function. Okay.
[57:19] So now let's print. All right, curiosity. Yeah. Why is it not printing this on, but it was doing that like I'm just curious.
[57:32] If I uncomment this and just say, Hello name what happens going to do it really quick and find out. Oh, there we go.
[57:52] Run without debugging. Oh, hey, it was because it was calling the function.
[58:03] Yay. So it's actually using the function.
[58:08] For those who are newer to teach gen tech. And yes, I am happy to see more developers on Twitch. Go follow Laura as well because she is also a developer on tech. I can't remember how to do shout out. I starting next week, I am actually going to be doing a database or data infrastructure. So we're going to have some main things that I do four times a week.
[58:41] Mondays are with Laura with Miss Monday, which is just fun, because we talk, we try to talk about other things that somehow programming always gets into it, which is, it's fun. And then on Tuesdays is all going to be about database infrastructure or data infrastructure I need stop saying database infrastructure.
[58:59] And then Thursdays is with distributed, where we are working on open source and co working and Fridays is either Python like this, or TypeScript, because I'm learning both. So it's a little bit of everything, and different ways of learning from different people and it's exciting. And I say that because I haven't streamed for a few weeks because I got a new job and it feels really weird to be streaming again, and but also lovely.
[59:34] Why do I always like try to mess up your name on here. Well, then, if it says the proper shout out. Yay, it did the shout out.
[59:46] Yes. So, so this is actually making sense in the fact that this is something that I think you are so right about that you called out earlier, like, out of context of function didn't make any sense whatsoever.
[60:04] Where now I'm like, because in, for example, like I've been building my website and I'm working on building like a new website that has like Jen Jenod calm, and then it has links to like Ivan, and then teach Jen tech, and then shit you don't want to talk about. And, like, to do all of that, you still have functions in there. I just don't think I ever understood that this is called a function.
[60:37] Indeed. So what I say that the function is from line three to line nine, or only line three the line six because that's what's included in the indent.
[60:51] Yes, it's the latter. It's line three to line six, that's the function definition. And then on line eight, we use the function. And so, in programming we call that like calling a function.
[61:09] You know what y'all, I'm going to ask. I'm going to take a little picture. We're going to take a picture of this. We're going to ask the Twitters, if they know what this is called.
[61:22] What do you think Twitter will say, I wouldn't know how to answer that question. Yeah, because it's out of context and I'm kind of excited about it. Well no I mean like, I would I would be looking at that and being like yeah what is what is like, what is it, well it's a block of code that contains a function.
[61:42] What is this block of code called? What is this block of code represent?
[61:53] If you're going to do that, it would be clearer if you just had line three. Maybe, because it's like a function definition. I don't know.
[62:07] I don't know. But actually, so I said something that was like sort of true.
[62:13] I said that line three to line six was a function. It is.
[62:19] But how many functions appear in lines three through six? Based on what you just said, I feel like you gave it away and it's just one.
[62:33] No, it's three. Three functions? There are three functions.
[62:38] So define the print and the name, because returning is I would think non-function, it just shows it. Name isn't a function.
[62:51] But it's getting what's going to be returned by the function input. It's a function whose name is input.
[63:05] Well, that might be one more time. Okay, so on line five, where you have input and then parentheses, you are using the function called input.
[63:18] Okay. Which is a built-in function in Python.
[63:24] Just like print is a built-in function. So return isn't a function.
[63:30] No, it's an optional component of a function. For Chrissy's question, and we're going to see if I got this right, I'm pretty sure a let would be for JavaScript where in Python we wouldn't need it.
[63:53] Yeah, so not just JavaScript. Lots of languages have that idea.
[64:01] But Python does not. What do you normally code in, Chrissy?
[64:09] I'm curious now. Interesting.
[64:14] And also, yeah, I will post this, Chrissy, later today, probably when we're done streaming and see how I'm going to phrase this. Maybe I'll put the code block and be like, hey, what is this code block called and how many of them are there in it?
[64:33] There is a let function -- you can do a let statement in Python, but you do not need to. I'm not going to confuse you by getting into that right now.
[64:48] I'm stepping off screen because for those who are newer, I still use books. I just have the computer read them out loud and then I take notes in the book.
[64:57] So I'm looking at the last chapter to see -- because I feel like in our summary it mentioned let. Let me look.
[65:11] It mentioned len in the first paragraph. That is also a built-in function.
[65:19] And len is short for length. And it returns the length of a string.
[65:27] >> Okay. >> Okay.
[65:36] >> I feel like I'm not going to lie on this one. I'm kind of like we also haven't streamed in forever.
[65:44] So the stream is like my brain process. Because now that I'm getting a function, I would love to reread this chapter for next time to see if I can understand it a bit more.
[66:03] Now that I'm finally conceptualizing what the function is, where it was out of context. >> Right.
[66:12] >> So for anyone that's joining a little later, what I do and Laura and I ended up doing and now I do it for TypeScript, too, is so we're using -- I always say his last name wrong. How do you say his last name?
[66:29] >> Swigert. >> Swigert.
[66:33] >> So we're going to automate the boring stuff. And so I use a screen reader or a text-to-speech to be able to read all of the text.
[66:48] And then I have the physical book where I will, on some of them, this is a good one, put lots of random comments and notes. So I remember where to associate them with.
[67:00] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[67:10] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[67:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[67:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[67:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[67:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[67:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[67:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[67:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[67:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[67:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[67:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[67:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[67:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[68:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[68:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[68:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[68:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[68:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[68:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[68:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[68:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[68:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[68:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[68:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[68:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[68:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[68:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[68:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[69:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[69:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[69:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[69:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[69:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[69:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[69:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[69:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[69:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[69:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[69:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[69:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[69:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[69:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[69:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[70:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[70:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[70:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[70:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[70:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[70:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[70:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[70:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[70:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[70:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[70:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[70:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[70:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[70:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[70:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[71:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[71:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[71:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[71:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[71:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[71:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[71:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[71:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[71:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[71:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[71:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[71:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[71:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[71:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[71:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[72:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[72:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[72:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[72:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[72:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[72:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[72:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[72:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[72:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[72:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[72:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[72:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[72:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[72:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[72:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[73:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[73:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[73:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[73:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[73:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[73:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[73:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[73:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[73:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[73:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[73:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[73:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[73:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[73:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[73:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[74:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[74:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[74:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[74:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[74:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[74:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[74:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[74:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[74:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[74:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[74:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[74:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[74:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[74:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[74:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[75:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[75:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[75:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[75:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[75:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[75:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[75:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[75:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[75:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[75:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[75:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[75:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[75:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[75:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[75:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[76:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[76:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[76:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[76:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[76:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[76:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[76:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[76:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[76:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[76:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[76:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[76:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[76:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[76:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[76:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[77:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[77:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[77:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[77:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[77:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[77:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[77:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[77:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[77:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[77:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[77:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[77:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[77:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[77:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[77:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[78:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[78:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[78:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[78:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[78:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[78:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[78:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[78:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[78:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[78:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[78:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[78:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[78:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[78:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[78:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[79:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[79:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[79:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[79:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[79:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[79:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[79:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[79:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[79:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[79:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[79:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[79:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[79:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[79:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[79:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[80:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[80:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[80:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[80:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[80:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[80:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[80:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[80:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[80:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[80:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[80:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[80:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[80:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[80:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[80:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[81:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[81:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[81:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[81:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[81:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[81:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[81:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[81:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[81:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[81:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[81:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[81:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[81:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[81:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[81:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[82:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[82:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[82:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[82:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[82:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[82:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[82:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[82:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[82:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[82:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[82:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[82:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[82:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[82:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[82:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[83:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[83:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[83:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[83:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[83:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[83:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[83:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[83:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[83:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[83:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[83:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[83:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[83:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[83:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[83:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[84:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[84:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[84:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[84:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[84:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[84:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[84:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[84:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[84:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[84:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[84:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[84:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[84:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[84:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[84:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[85:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[85:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[85:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[85:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[85:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[85:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[85:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[85:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[85:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[85:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[85:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[85:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[85:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[85:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[85:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[86:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[86:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[86:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[86:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[86:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[86:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[86:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[86:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[86:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[86:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[86:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[86:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[86:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[86:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[86:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[87:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[87:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[87:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[87:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[87:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[87:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[87:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[87:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[87:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[87:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[87:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[87:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[87:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[87:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[87:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[88:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[88:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[88:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[88:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[88:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[88:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[88:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[88:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[88:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[88:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[88:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[88:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[88:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[88:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[88:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[89:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[89:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[89:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[89:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[89:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[89:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[89:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[89:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[89:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[89:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[89:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[89:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[89:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[89:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[89:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[90:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[90:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[90:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[90:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[90:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[90:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[90:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[90:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[90:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[90:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[90:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[90:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[90:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[90:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[90:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[91:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[91:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[91:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[91:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[91:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[91:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[91:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[91:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[91:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[91:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[91:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[91:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[91:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[91:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[91:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[92:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[92:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[92:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[92:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[92:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[92:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[92:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[92:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[92:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[92:39] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[92:43] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[92:47] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[92:51] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[92:55] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[92:59] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[93:03] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[93:07] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[93:11] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[93:15] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[93:19] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[93:23] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[93:27] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[93:31] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[93:35] And then I will have a screen reader and a text-to-speech. And then I will have a screen reader and a text-to-speech.
[93:39] And then I will have a screen reader and a text-to-speech. 
