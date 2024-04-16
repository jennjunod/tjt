---
showLink: "https://www.youtube.com/watch?v=mCGSFnroX4Y"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-data-basics-and-caching-with-guest-ben-gamble"
title: "Teach Jenn Data Basics and Caching with guest Ben Gamble"
publishDate: "2023-04-14"
coverImage: "https://i.ytimg.com/vi_webp/mCGSFnroX4Y/maxresdefault.webp"
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

[00:00] to another episode of Teach Gen Tech where we have Ben back again and I'm excited 'cause we are learning the basics of data because, well, we use data day in, day out. You just
[00:15] watch the stream, hear the stream, do anything about on the interwebs. It all uses data. And Ben, I feel like I should know a better introduction for you, but you're Beth Gamble
[00:29] that does absolutely everything and currently is a dev rel at Ivan as well. But what's your official introduction?
[00:39] So these days I mostly go by the open source technology, which is kind of as a joke based around my job, mostly being about pairing some Kafka, some Postgres and maybe some cheese
[00:49] in the middle. And the idea of basically trying to pair the right pieces of software to build that stack. And the reason about this is that these days, most of what you do is no longer
[01:00] just that single column of tech of your server, your database, and maybe a web framework on top. These days there are more bits in the stack. Therefore, you've got to pair the right
[01:09] pieces together to get the best outcome. Yes. Yes. All of that. All of that.
[01:15] Also, it's a good joke. And I feel like that's such a good thing because as I've been learning about databases, especially
[01:25] Postgres right now, a lot of it is I'm seeing how much it's interconnected with everything else. Everything is connected. It's just learning what they are and how they're connected, which
[01:39] has been fun and annoying. The deeper you get into this, the more you get this kind of weird dichotomy of everything
[01:49] is different, but everything's the same, but it's all very different, but it's all the same, but it won't talk unless you really make it.
[01:57] And this is something that I've been realizing with learning live in the last nine months has been things that are very, very complex can make total sense until you go to do it.
[02:11] And then it doesn't make sense at all. And you're like, what? What? So that is what I have realized that I get really stuck with. And I have linked in the chat, y'all, the
[02:27] playlist from that I started about this series, which currently just our last episode. Eventually, I will also link in the Postgres ones, because they're also learning about data. Yeah. Anything
[02:42] you want to go over before I show you recaps of last week and where I got stuck? I think that's really everything, really. To be honest, other than the playlist is great.
[02:54] Please watch it. Yes, yes. And I feel like so yesterday, I had a friend on his name's Anthony Campolo,
[03:06] and he was on and he works for Egeo, which is a part of Limelight. And I had no idea that his friend Scott was part of them until they started saying that there's their Twitter
[03:21] space every week is a part of Egeo. I was like, oh, anyway, all that to say that Scott is the best at doing his radio ads of make sure that you follow everybody on the screen
[03:35] and in the Twitter space and to like, follow and interact and make sure to come on stage and ask questions.
[03:41] You really ought to get a difficult soundbite for this and then press the button. Oh, that. Yes, yes. That is what I should do. And OK, well, going to our lovely data
[03:58] spreadsheet, which y'all been did a lot of this work before our stream last week, and I copy and pasted and wrote notes about some of it. So I'm going to go through and see
[04:12] what I remember and get corrected on some things. So because you mean, hey, this is where we started when we were talking about how data progresses, which and the speed of
[04:30] progression where like when you have a cache, it's the very, very first part of where data starts. It's only in the single digits of megabytes. And we talked about how a thousand
[04:45] twenty four megabytes go into a gigabyte. I almost feel like I want to go over here. We're going to postpone just a moment. Because would this help knowing the rest of them going
[04:57] through this first or does this make it more confusing? So this is really about speed. So this is like so this is where the best thing to do
[05:03] is actually start where we were. I think I can run the quick recap as well. So go back to where we were. The main thing to do is start. Yes. So the best start here. So the
[05:17] key thing to start with is CPU in your machine can only act on a few bits and pieces at once. Those bits in the cache, which is both the fastest and the most expensive piece of memory.
[05:26] When you need more data, you pull it from what's known as main memory or RAM, random access memory, which is nowhere near as costly and as a separate normally a separate chip
[05:36] on your machines or your CPU. And that's kind of measured in like gigabytes. You have gigabytes of RAM. You can go up to terabytes of RAM just about these days, but you're going to
[05:45] be paying a lot of money for that. Cache is single digit megabytes to about 30 megabytes on a big CPU. You don't get much cache and it's very, very expensive to get more.
[05:57] So then as you go down again, we get to your kind of persistent storage because RAM is still what's known as volatile. You turn the machine off, it's all gone. And these are
[06:06] where you get SSDs and hard disks, spinning platter drives. And these are not slow by any stretch of the imagination for what comes next, but they are much, much slower again,
[06:18] but also much, much bigger than RAM. After we get to the disk drives, we kind of go beyond the size of what one machine will hold. And this is where we get to this kind of like
[06:26] what often is referred to as like cloud scale stuff. So we go, okay, so our local area might have like four or five machines all stapled together using the local area network LAN.
[06:37] And that will give us all the different disks attached to all the different machines to access. That's great. But now if you imagine that cables go machine to machines, and now
[06:45] your band is now your kind of finite max speed is, I've got a call over there. It's physically further away. It takes longer for the data to get there. It's not that slow by comparison
[06:55] to the next step, which is the wide area network or the WAN, which is, I would use S3 or equivalent or some of the block object storage, which is no longer on the machines you probably
[07:04] own, but is if you own them on-prem, but they're so far away by comparison. There's so many of them that it's once again, much, much, much, much bigger. You can store exabytes
[07:15] of data in S3, but you know, the access speed is going to be commensurately lower. There are some good trade-offs and bad trade-offs there, but it's so cheap by comparison to
[07:25] your cache or your RAM, or even your local hard drives, it is very much worth the trade-off if that's what you can get away with. The kind of really important thing to know is
[07:36] that eventually if you want to act upon that data, it does have to hit your cache at some point, or your CPU can't touch it. This is like, if you imagine a production line, like
[07:46] the machine itself has, like where the thing, the stamps, the stamps out like a punch into a piece of flat metal. That bit we can act upon is your cache. It's a very small area,
[07:57] but then lots of bits can go through. So you've got to pump them through the cache to get things done. And that's kind of the core of what we started off with. And that's why you
[08:06] get the kilobytes, megabytes, gigabytes, terabytes, and petabytes. It's just kind of like, as you go down, you get bigger, cheaper, and slower. As you go up, you get much more expensive,
[08:15] much smaller, and much, much faster. And this is where we then jump to that lovely little diagram about latency, because this is like where it ends up being important. Because
[08:27] latency is just the time it takes for something to happen. Right? Yes. Yeah. I ended up somehow merging some of the notes, but I'm moving this over so
[08:40] we can see both. Yeah. The other direction. Because buffering did help when you were talking about the water. Yes. So these are my lovely graphics to go with it. Now, one thing that
[08:56] helps for me to remember when I'm looking at these is, for some reason, some words just don't click. Like that RAM and memory are the same thing. Why? I have no idea.
[09:07] Random access memory. So I wrote it out. And CPU and GPU is similar. But do most computers have both? Or does the GPU use or is inside of the CPU?
[09:24] So these days, they are nearly always discrete pieces of silicon. However, they might be built in. You can get a piece of-- a GPU chip is often built into a CPU. So Intel have what's
[09:38] known as integrated graphics, often. And those are integrated into the actual same piece of silicon. But they'll still be a separate area. But it will be integrated onto the same
[09:51] piece. Say, wafer or dyes is often known. AMD does this as well with their, what's known as APU range of processes. But it is increasingly common in some places and uncommon in others.
[10:10] When you get to specialist hardware, as in hardware which has performance characteristics, you tend to have discrete units. So there's a discrete GPU. Because then you get all of
[10:20] the usefulness of lots of space and good heat management. If you imagine you wanted to have a beefy game running high speeds, you don't want to have all the heat that generates in
[10:31] the same place as your CPU. Because you can imagine the load is a lot higher. That makes sense. So thank you for those clarifications. That does help. OK, now I have to--
[10:46] Maybe one kind of thing to make is as you go in, the problem ends up being that a lot of what we consider computers to be is still based off a bunch of thought processes left
[10:57] over from the late '80s to-- early to late '80s of what I would call the PDP-11 era of thinking. And what that means is, all of our various mental models, often the way we actually
[11:12] program, are based around a bunch of these computers that no longer exist. Back when it was so prohibitively expensive to do some things that decisions were made.
[11:22] So what that really means is, as you come to today's actual chips and hardware design, so many things are-- it depends out of the box now. Because I could tell you about specialist
[11:37] pieces of hardware where they're mostly GPU, a tiny bit of CPU. You could literally get something called an FPGA, which can then just put all the different bits in one piece of
[11:46] silicon and do all kinds of nonsense. But it basically is because we've gotten so good at building hardware, in some respects, that we've specialized and then generalized and
[11:58] specialized and generalized a couple of cycles over. So everything has become that weird-- if you imagine all the dog freeze turning into mongrels, that level.
[12:07] OK. So it's a little bit strange over time. But I'm still going to go by the generalities
[12:13] we normally use, because they still hold true more often than not. OK. And that is making sense. Everything you're saying there makes sense. I now get why you
[12:25] were saying to go to this second. So thank you. So it does say-- So this is not a second to start with.
[12:38] Yeah. So I guess the other part that-- and this is a big reason, A, I'm super glad that we're doing this again. But also that I'm writing notes as we go, is I've realized it's
[12:50] helped me learn so much better. Because people can fact check what I'm actually writing down. It's marvelous. So when we're talking about 1NS, this is what Cache is using.
[13:03] Yeah. So Cache-- so the first one there is that the L1 Cache reference is half a nanosecond. This is about one CPU cycle. I can't remember how many CPU cycles this is, because it depends
[13:15] too much on things. But fundamentally, half a nanosecond is about the fastest thing a CPU will do. Then these are all inside Caches. So L2 is another bit of the Cache. It's just
[13:23] a bit-- because Cache is at levels, but not really important for today. The key thing really here is you're looking at tens of nanoseconds-- below 10 nanoseconds to do things from Cache,
[13:36] really. Below 10 nanoseconds. This is one thing I'm learning with the AccelerDraw, is it can still pick up my pencil so much
[13:48] more, that I cross out my-- so you said single-digit nanoseconds? Yeah. Single-digit nanoseconds is your Cache stuff. So everything in Cache is single-digit
[14:00] nanoseconds-ish. And these are mostly orders-- the way to think of this is it often ends up being a bit-- it's a bit hardware-dependent when you get down to these low speeds, really
[14:13] fast things. So these are just-- it's best to think in terms of tens of, hundreds of, thousands of digits of, for this stuff. Because you'll get a lot of people go, well, actually,
[14:25] blah, blah, blah, blah, blah, blah, blah. And that doesn't really matter. For most practical use cases I know of, and nearly all the engineering I've ever done, including hardcore handwriting
[14:39] in the assembly stuff, an order of magnitude of time units is all you'll ever need in kind of resolution. I've only ever come up a couple of times when we talked about actual exact
[14:51] nanos. OK. Now that we went through a bit of the beginning part again, what would you say--
[15:01] so we talked about that Cache is megabytes. And now we're talking about that Cache is nanoseconds. So it's how long it takes to process.
[15:13] To do something. To do something, yeah. Nanoseconds to process.
[15:17] Cache actions, yeah. An action from Cache takes nanoseconds. The reason I say action is because it's a bit vague when it gets into the Cache of what you're actually doing. And
[15:28] I've tried-- the general rule is, yeah, using stuff from Cache is nanoseconds. OK. So cool.
[15:35] And then the next one up is RAM or main memory. So RAM, of course, is random access memory. And this is where I talked about the computers from the '80s, because RAM is often specifically
[15:49] used to differentiate from ROM, which is read-only memory, or EPROM and other things like this, where this is memory where you could basically flash it once, and it would hold whatever
[16:02] you gave it. OK.
[16:04] And you could never write to it, but you could keep reading from it very quickly. So main memory reference-- this is accessing something in your main memory-- is hundreds of nanoseconds.
[16:17] So you've got a RAM for 100 nanos or more. So 3 digit nanos. So this is random access memory, not read-access memory.
[16:27] Yeah. OK.
[16:29] Read-only memory, yeah. So RAM, not ROM. ROM is not relevant in today's-- in today's world of what we do. I wish I could say ROM has not come up in my career as a thing I need
[16:41] to deal with, but my career is otherwise known as I do nonsense. Yeah. That's one way to put it.
[16:49] So-- oh, yes, yes. People pay me for the nonsense. OK. If this one's reading-- OK, cool.
[16:57] Access memory. And I think that's why I'm also getting ROM is read-only memory.
[17:07] Yes. So this is a useful thing to know, only because it will help understand the acronym, right? And the problem with this stuff is always that a lot-- it's like the idea of--
[17:17] there are people who think a floppy disk picture is just a save symbol, not representative of a disk we used to physically have.
[17:25] Yeah. It's the-- like, there's a lot of problems with computing, is computing is now old enough
[17:29] that things have gone-- and it changes so quickly, that things have gone obsolete that used to be so core to what we do that their names or their pictures persist so much longer
[17:39] than the actual thing themselves. Yeah. Yo, what up, Lex? As you can see, I was probably way too focused on writing notes.
[17:48] And yay, Lex has been learning along with me. I found out yesterday that the way I explained Docker and Kubernetes in basic terms made sense to somebody else. I was very excited.
[18:02] It took me ages to get my head around, like, why that kind of virtualization mattered. Like, I don't mean ages. Like, it was, like, a couple of years into using it before I was
[18:11] like-- it finally clicked of why this was relevant. Oh, I don't-- that, like, makes sense to me. But then there's, like, this kind of stuff
[18:19] where I'm like, why can I not get it? So I suppose this is the other classic thing of, like, this is where I started, like, at
[18:28] this kind of level of, like, bits on wires, versus you started probably with more complete systems. And it's just-- all it comes down to is, like, your entry into this world comes
[18:37] from one side or the other side nearly always. So you either know-- you know some stuff you don't know others. Because there's just too much to know now.
[18:48] I'm trying to think what SSD is. Solid-state disk.
[18:53] OK. Solid-state disk. So this is differentiated from what's from the old hard disk drives, which were spinning.
[19:03] Because they actually used to spin, of course. So they don't spin, because they're solid. No moving parts in an SSD.
[19:16] And this is kind of noticeable, because if your disk was in a particularly bad state, you'd hear it going tick, tick, tick, tick, tick, which is the head moving around, the
[19:30] read head moving around, and occasionally hitting on the disk itself. Oh. Lex, I am going to be starting a new database next month sometime. And I think I'm going
[19:45] to be building Raspberry Pis. Yes. We actually have some of them here, which we're going to be using for this.
[19:53] Yes. So, Lex, I'm going to need to make sure that you're in the audience when I get stuck. OK. Cool. And I also put a few more notes of, like, solid state, just so that way I
[20:07] knew the difference. And I think something that I might have missed last time was the fact that RAM erases when it's turned off, where solid state saves it.
[20:24] Yes. This is actually one of the more important distinctions. So there's a whole line I could follow about. It depends on, well, actually, but that's not important today. What's important
[20:36] today is that, like, this is why a lot of tools like Kafka and Redis are often, so things like Kafka is quite important, because everything in Kafka, once you've got the acknowledgments
[20:48] back, have been written to a persistent disk, which is like an SSD. And where we work at Ivan, all of our machines have attached solid state drives. And so every time a Kafka message
[21:03] comes in and it's saved to that disk, it means it won't go away if the machine is turned off. So that, therefore, is what's known as a durable write. So this is where the terms
[21:11] durable often come in. So durable data means that it'll survive a machine getting powered on and off, whereas ephemeral data doesn't. So Redis is famously ephemeral most of the
[21:25] time. Because Redis is all in RAM. >> Okay. This is not proper. You know what? I feel like it'll at least help me keep my memory when I get there. And I will ask you
[21:41] about what you just said in a bit, because I feel like I could go to a tangent on that. And then we have is this last one? I don't know why I'm looking on my tablet. >> This
[21:52] is network-attached storage, really. >> So like AWS. >> Basically S3 or -- I just call this network storage, really. Because it could be almost
[22:04] anything. >> What -- okay. So network -- what? >> Network storage. So these days it's nearly always what's known as an object store, which is something like S3 or Azure object store
[22:19] or DigitalOcean has one. Did you just delete something? >> Yeah, and I don't -- oh, I found my undo button. Thanks. Sorry. I was looking for the undo button. I got it. We got there.
[22:30] >> The point really is that -- to make here is that this is data on a different machine now. That's why I always refer to it as network storage. Because to be honest, it could be
[22:41] almost anything. Right? But it's just -- it's data on another machine. So network-attached storage. So S3 is a magical thing Amazon have built to give us access to near unlimited
[22:57] storage. Then everyone else, of course, has their own equivalents. If you go back five plus years, this would have been -- we'd have used something called HDFS to do exactly the
[23:06] same thing. But we'd have to run that ourselves. Classically, this was just a big -- just a remote disk access to a machine some place far away. And the reason why this is important
[23:21] is like what you've -- what we're now saying is mostly just how long things take. So if we go back to that kind of black, blue, green, and red, right? And a random read on your
[23:35] SSD was about 150 microseconds. Right? Now, let's say you're going to read something from a disk quite far away. So now we're 1,000 times slower to go to, let's say, to go from
[23:48] California to the Netherlands. And now what happens is once we get there, we have to do the read, which means it's got to go through an SSD read. And then we've got to go and
[23:56] send it back again. So you've basically got -- you're literally 1,000 times slower to read from S3 than it is to read from your local machine.
[24:06] And okay. So that part makes sense. What are external hard drives considered? Like, I know they have some SSDs, but then they have HDDs.
[24:19] So an external drive could be anything in a box. Like, you know, your flash drive, pen drive could be one of those as well. For all intents and purposes, it is a network-attached
[24:29] storage device, except the network is very small. >> Okay. That is helpful, though. >> So the main thing to understand here is
[24:38] I'd say a big reason that takes 150 milliseconds to get from one place to the other is the speed of light is only so fast. Right? So the light -- literally the electrons take
[24:51] a little bit of time to go from one place to the next and back again. So if they've only got to go to your pen drive, which is plugged into your USB port, that doesn't take
[25:00] very long, by comparison. >> Okay. So totally getting this now. So okay. So the network-attached and, like, the external drive, totally starting to make sense, I guess.
[25:24] And I think this is going to lead us somewhere else. Then where does AWS and those type of things come into it? Are they the same as network-attached, as, like, GoDaddy hosting
[25:36] server? >> For all intents and purposes, yes. So if we scroll a little -- so I'm going to scroll over to one of our earlier diagrams again,
[25:47] which is the one -- straight down, actually. Just straight down. So what's going on here, right, is the idea of, you know, you're loading data into your CPU from your drive, right,
[26:01] your SSD, and then you want to go to S3, so there's a network hop to a different CPU somewhere else, right? And then you're loading -- they're loading from their massive pile of much cheaper
[26:12] SSDs or tape drives or whatever else they're using. It doesn't really matter. They've got all their storage on their own machines, and they've got to load it, put it in their CPU,
[26:19] and send it over the network to you. Now, let's just say for a second that we are, I don't know, downloading a file from GoDaddy, right, for a GoDaddy hosting web page, right?
[26:30] I say, "Give me that file." That sends a ping over, and then that file starts to download. For that file to download, the web server running on GoDaddy has to access the storage
[26:39] in GoDaddy, right, and then start sending me the file. >> Okay. >> All over the wire, right? So that's some
[26:47] CPU operations, then it reads from its SSD into its CPU, then flaps it over the wire to me, and then it's read in over my network into my CPU, then written to my SSD. Dependent
[26:59] on some stuff, but for all intents and purposes, that's what happens, right? >> Right. >> And the whole point here is S3 is just someone
[27:09] -- once again, this is the main thing about the cloud and everything in the cloud is it's someone else's computer, right? Or someone else's big, big, big pile of computers. Or
[27:22] in the case of S3, a very, very -- a comically large number of machines running in a comically large number of data centers with, frankly, ludicrous levels of redundancy, allowing you
[27:34] to basically read blocks of data at near random access surprisingly quickly. So necklace-attached data, and this is just a catch-all term I'm using, because it could
[27:51] be anything. Like, back in the day, when you just hosted your own little web server on a machine somewhere, you might have a single U1 rack in a data center where you've literally
[28:04] walked up to the data center, plugged in your rack, plugged in the cable, and be serving from that directly. That meant all the data your website could serve came from that rack.
[28:14] But as a user, that's remote disk storage, effectively, which you're accessing. >> Okay, this is -- this is starting to make so much more sense.
[28:25] >> So the golden rule here is that most things are weirdly the same when you drill -- when you slice enough layers off the top. The problem -- there's a lot of, of course, very important
[28:37] details which we can slightly ignore for today, because genuinely, they don't change much, because fundamentally, they have to work this way.
[28:46] >> Okay. >> If you think about it, there has to be a computer at the other end. So I say give me
[28:53] file X. And AWS has got to have something that says, I know where file X is. Here it is. So it has to be a computer.
[29:02] >> Right. And that's all making sense, because this is also starting to make more sense as we go into -- like, yesterday, Anthony was on the show talking about Docker. So this
[29:14] is making a lot more sense with Docker as an example of whatever this red box is. Now -- and this might be taking us off on a different tangent, but, you know, this is the fun part
[29:27] about teach gen tech. We kind of have a goal, and then sometimes we just go off on different parts.
[29:33] >> Yes. >> So we are taking it to the network. Taking it off of the network. Why is it going from
[29:41] the SSD to the RAM to the CPU instead of vice versa? >> Okay. So this is merely because I drew it wrong. If I correct my drawing for a second
[29:54] here. So this is merely because of the way I drew it. So what really should happen here is if I can remember where my controls are, please keep the right settings right. So let's
[30:05] draw this box, which needs a little bit of fill, because the fill is really pretty on this. Right? And let's call this -- because this is where I get in trouble for oversimplifying
[30:16] things. >> I'm going to move all of this stuff above here. There we go.
[30:21] >> So this is where the level of abstraction kind of comes to bite me. Zoom in. And zoom in. There we go. So if I make this a bit bigger, I make this a bit bigger to go with it. So
[30:38] this is the network device. The machine has a physical device which handles the networking for it. Right? So if I load -- if I want something from the network, right, I load it like this.
[30:51] Right? Because it's a network device. And this is going to probably go directly into -- network device basically goes via the CPU like that.
[31:02] >> Oh. Okay. >> So what happens here is -- so let's say you start loading data on your local machine
[31:08] off the SSD. Now you want to load data off the network. So you go -- CPU says to the network device, go dial S3, give me some data, please. Or basically if it has a get request,
[31:19] the get request hits a video, right? So that goes over the network device to the CPU of the other machine and says, I want this video, please. It goes, okay, send it. Pulls it off
[31:28] the SSD pile at the bottom, right? And then loads that through RAM, through the CPU, and it buffers it into the RAM and sends that from the CPU through its network device to
[31:38] this network device which beams it and the CPU then goes, what should I do with this? Basically buffer it in RAM. And then once it's in RAM, read it back to the CPU to play
[31:47] that video we were talking about. Because effectively, your red box is missing. What's missing previously is that red box you just drew for your machine. So if you draw a red
[31:59] box around all these boxes above loading over the network -- >> Yeah. Well --
[32:06] >> Because that's your machine. >> Let's start with the red box because that actually simplifies things a lot.
[32:16] >> Well, is the CPU the brain then? >> Yeah. It is. Literally. It's often described as the brain of the machine. Everything goes
[32:24] through the brain. >> I think this is helping. Hold on. Let me draw this out to see if this is actually accurate.
[32:31] Okay. Yay. That's not -- >> So with RAM, if I'm watching a YouTube video, it's using RAM but it's not going to
[32:58] use the SSD because I never downloaded it. >> Yeah. Exactly.
[33:02] >> Ah. Okay. I'm getting there. I am getting there. >> And the reason why it holds on to it for a little bit is Chrome says I'm going to hold
[33:10] on to -- even though you just closed that tab, I'm going to hold on to that RAM for a little bit longer until 100% I'm sure you're done with it. So if you notice, I've just
[33:20] drawn a box around the outside of this, right? >> Yes. Yes.
[33:23] >> This is your machine. >> Hi.
[33:26] >> This is the network machine. >> The stored -- and browser cache. But that's not the same as CPU type of cache.
[33:50] >> No. It's -- so this is the other classic problem. All the words are used for everything. So a cache is -- so the problem is -- so this is where we normally refer to it as L1 cache
[33:59] or something like that. Because Redis is a cache. Your browser cache is a cache. Your SSD has caches built straight into it. There are caches everywhere.
[34:08] >> Why? >> And the short -- why? Well, because of what caching is for, which is that everything
[34:14] is slow, therefore we cache. As in, we don't -- as in, it's cheaper to hold the data for a bit, the data we think we're going to use next is to try and fetch it again from zero.
[34:27] So it's the other classic thing of why do we save bits of the web page? So why do we cache bits of -- let's say we hit -- let's say we go to, I don't know, LinkedIn, twice
[34:36] a day, right? So all the LinkedIn assets are actually saved in your browser cache, right? Because it's much better to hit a hot cache which has data in it than it is to load it
[34:47] over the network. You could load it over the network every time, but then it'd be slow. It'd waste literally tons of stuff. Like, why waste the power? Why waste the internet?
[34:56] Why waste the bandwidth? And why waste your time? So that's why we cache stuff. And it's exactly the same. It's like, why would your CPU not hold whatever it could in cache to
[35:05] act on that there and then before it has to go fetch another chunk at a time? So caching is basically picking up -- this idea of saying, I'm going to go -- I need
[35:15] to -- so I'm going to pick up a carrot, take it over to the bench, chop it, and I'm going to pick up another carrot, rather than going, I'm going to pick up five carrots, bring them
[35:21] over to the bench, and then cut them up. Because my cache is my bench space is enough to have at least five carrots in it.
[35:32] Okay. It's stopping round trips. Caching is all about reducing the number of round trips you've
[35:38] got to do, because most things happen more than once. And this is making sense. So is cache the same as buffering, then?
[35:50] Yep, that's the same thing. A buffer could be called a cache. Sweet.
[35:54] Quite literally. I am putting two and two together now.
[36:00] In fact, I'd go one step further to say a buffer is a specialized single-purpose cache. Oh, okay.
[36:12] Because a cache can be anything. But generally, if you buffer something, you're buffering one specific thing.
[36:20] Whereas a cache can have many different things in it. This is a -- this might be a semantic argument you might cause, though, but I will happily
[36:32] stand by that for now until proven otherwise. If I'm wrong, reach out in the comments.
[36:43] I'm asking because this is making a lot more sense in the fact that now when I go back down to my examples that I was working on, like, reading earlier, it's making a lot more
[36:55] sense how we're going from place to place and what places are used for. Yes.
[37:01] Oddly, I think a lot of it had to be, like, you had to go through this the first time last time, and then I needed to go through the same stuff again to ask more questions.
[37:11] Because this is seriously helping. I think --
[37:16] So -- Oh, go ahead.
[37:18] No, so this is kind of -- to go back to the database thing, so Postgres has caches built into it.
[37:25] So if you do a query in Postgres the first time, it takes a long while, but if you do exactly the same query immediately after, it doesn't take anywhere near as long.
[37:32] Because it's still holding the result. And when we talk about query, are we talking about, like, if we say -- if we go to the
[37:40] Spice Girls example from the last episode, let's say we are looking for things with Scary Spice.
[37:47] Yes. Would it be considered the same query if I look for things with Baby Spice?
[37:52] No. Or is that a new query?
[37:54] Okay. That would be a new query.
[37:56] But let's say both you and I were looking for songs by Scary Spice. So my query landed first.
[38:02] It took four seconds to come back. This is an arbitrary amount of time, just an amount of time, four seconds.
[38:07] That was slow. However, you then queried after I did and asked exactly the same thing, songs by Scary
[38:12] Spice, please. But because there's a cache in there, it goes, someone just asked for this.
[38:16] Here is your answer. I don't have to go search for it again.
[38:20] Even if we're in different locations? Yes.
[38:23] Because it's the same database. Interesting.
[38:25] Interesting. So that's what caching is all about, really.
[38:31] The idea of caching is to say the same thing, it's very rare that things happen exactly once.
[38:37] It's quite common things will happen more than once. And a lot of cases, the same thing tends to happen over and over and over again.
[38:44] Now we have a lot of tools which are optimized for these various access patterns. And access patterns really determine what tool you use in a very real way.
[38:55] So whether you need to keep your data in RAM, or can you keep it on disk, depends how you access it, or why you access it.
[39:01] And this is where everything from your database choice to how you build it matters. So if you think about some data of, let's say, back to the video, I want to access this
[39:17] video. Right?
[39:19] So this video is probably going to be a big-- it's a big file. It's going to be stored in chunks, and I'm going to keep it on my disk.
[39:26] Right? And I might have a little index file that tells me how far along that video to go to
[39:31] get to, let's say, the chapters, like chapters in the video, or the key points in the video. But fundamentally, the video doesn't make sense unless you read it in order.
[39:41] Because it's a fundamentally time-ordered thing. So the only way you search it is time, really, in video.
[39:48] But back to our discography, right, of the Spice Girls, there's various things you want to search on.
[39:54] But also, it's very likely that the amount of data you want from that thing is very small compared to the total amount of data.
[40:03] So you want to be able to query and get a bit back, rather than saying a video, where it's very likely you're going to watch all the pixels in the video.
[40:09] OK. Think about it.
[40:12] Yes. I feel like I-- and I just wrote this down.
[40:18] There we go. Apparently, it's going to be giant.
[40:20] That's cool. So when we talk about a floppy disk, or a CD, I don't know if external hard drive goes
[40:27] with it. Yep.
[40:29] Would those-- I get they're technically network-- I would consider-- for the sake of this, we're going to consider them network-attached.
[40:38] Because fundamentally, there's a wire going from your machine to the device, which then has to read something.
[40:44] But they don't use RAM, because they're not randomly erased. They use--
[40:50] They're a file storage-- so this is where we-- the term here is a storage media. Aha.
[40:58] OK. Cool.
[41:00] I'm still going to put it in red, but-- We're good.
[41:02] No, it's always good. So the different storage medias you have are things like a floppy disk, a CD-- an external
[41:07] hard drive is just a hard drive in a box-- or a flash disk. Like your SD-- like an SD card.
[41:15] These are all the same kind of thing, if you think about it. Which is a device external to your machine, which stores data for you.
[41:25] I consider them network-attached, mostly because it's a very convenient way to term these pieces of tech.
[41:34] They can-- as per always, analogies start to break down when you get into specifics. So if you're ever using a floppy disk, it might as well be considered network-attached
[41:44] for the speed. Fair enough.
[41:46] I still have a floppy drive, which is quite fun. I had to go buy an external hard drive-- or external CD driver, because health tech is
[42:00] not up to date with the rest of the world. So when I go get my MRIs done, they give me a CD.
[42:06] Or I have to wait, like, weeks before I get the results back. So--
[42:11] I can believe that. Yeah.
[42:13] So I went and bought one. And I'm like, well, now I have it.
[42:17] So I think this is also really helpful. Again, going to go a totally different direction.
[42:23] Always good. It's so fun.
[42:25] It's so fun. OK.
[42:28] So we have file storage media, which this makes sense when we talk about these devices and we talked about Spice Girls, all that.
[42:38] What doesn't make sense now are projects, like I want to build a Astro website or something, because they all start with one folder.
[42:55] And then they are a file storage, and they have structure. Yep.
[42:59] OK. So I guess I'm not-- I get it, but I don't get it going from A to B.
[43:05] OK. So you're in that weird kind of space where you see a project directory, which has all
[43:11] your files in it, right? And what happens next?
[43:14] So the key thing, really, here is what your machine can-- so this is where we actually hit the other path.
[43:23] So there's more than one way things work in a CPU, just because of-- nothing can be simple because we're not allowed nice things.
[43:31] No, it's actually-- it's not too bad. So this is where, if you learned to program in the early '90s, this would have been--
[43:39] you'd have been taught this first, and you would have been wildly confused at the time, because that's how they taught programming back then.
[43:45] OK. It was very frustrating, which is the idea of the program counter versus the execution
[43:52] stack. So what's going on right now is, if you imagine you've got your Astro files, the first thing
[43:56] that happens is, we're going to assume there's a program running, right, which is the interpreter. Your computer goes, I will load this file into RAM, then it'll throw it into the node
[44:08] interpreter, it'll chew it up and spit out a series of what's known as intermediate representation, which is just another file with a very different shape, and then it'll basically follow the
[44:19] instructions written in that file, right? OK.
[44:24] So basically, you load it, and then what happens is, all the different function calls you've described, all the different states you've described, are turned into executable code
[44:35] on the machine via this program call, which is the interpreter. What happens-- the important thing to note is that you have all this project structure,
[44:47] and fundamentally, the structure is mostly there to make your life easy, not to make machines' life easy.
[44:53] What the machine does, it takes all your files and all your folders and munges them all together into one blob.
[45:00] I kid you not, that is normally how these things work, right? Because fundamentally, the machine just tags these as a series of objects in what's known
[45:07] as an abstract syntax tree, where it basically builds a diagram for itself-- a diagram is not really-- but it's basically a diagram of all the blobs in your code and all the
[45:17] flow paths. A massive flow chart, right?
[45:19] Yeah. So you have all the various states your system could be in, and then how to get to there
[45:24] from there, from there, from there, from there, right? And then you say start.
[45:26] You go to the first box, which is your main function, effectively, and it says, "Do this thing."
[45:32] Now, with Astro and tools like that, there's a whole ton of extra code, which is loaded behind the scenes in the library that makes Astro work, right?
[45:40] Okay. So if you imagine you load-- so it's actually a bit easier-- it's easier to start this from
[45:45] a different language than Astro. Astro is about-- it's about as far removed from--
[45:49] Well, really quick, for the executable, and it reads it, is that just the OS, and is that part of the CPU?
[45:59] No, no, no, no. That's-- I wish, but we're too far-- this is a problem.
[46:03] So we are a few levels up from that. So what's happening is-- if we scroll back a bit, that a lot of more simple programs
[46:12] are written in C, where-- remember in C, you have int main, and then some stuff, right? Mm-hmm.
[46:19] Right? So int main, then just say, you know, printf, "Hello, world," right?
[46:23] Okay. And then you close the braces, and that's it.
[46:25] So that little program there gets compiled down to machine code, effectively, which is what your executable is, right?
[46:32] Executable is machine code, which you basically-- when you double-click on it, that gets run by-- the OS says, "I know what that is."
[46:38] In Linux, that's called an ELF binary. In Windows, it's an exe file.
[46:42] In Mac, I do not remember the actual extension name anymore, but DMG, I think. Yeah.
[46:48] I think you're right. I'm pretty sure it's DMG.
[46:51] Yes. It might be.
[46:53] I can't remember. I can't remember.
[46:55] I can't remember. So what happens next is that the OS basically says, "Run" to that executable, right?
[47:06] And it basically starts feeding it to the CPU via the instruction cache, which is another cache.
[47:13] We've been talking about data caches so far, but there's another one called the instruction cache.
[47:17] Right? I know.
[47:19] It's annoying. I was hoping we could avoid that.
[47:21] It's fine. But it doesn't really matter.
[47:23] Now that I know there's a ton of them, it's starting to make more sense. So we're good.
[47:27] Yeah. So if you imagine there's two tracks of things flowing through the CPU.
[47:30] One is the instructions saying, "Do this, do that, do this, do that." The other is the data of things to act upon.
[47:36] Yeah. Okay.
[47:38] Right? So that's what your executable is, a series of machine code, which goes in the instruction
[47:42] cache, and the data it needs to operate on goes in the data cache. Now that's level, that's kind of like on the metal-ish stuff in C. Now in your Astro example,
[47:52] what happens is there is a piece of code that does that, but it's not bigger and it's called your interpreter.
[47:56] And what that does is says, most people don't have time to write all this stuff out in C or equivalent languages or Rust, and says, the assumption is that we'll give you a different
[48:08] language to write in, which gives you more powerful objects to work with and more flexibility to work with.
[48:16] Which is, you know, you can write four lines of node code, which would take a thousand lines of C to write.
[48:22] Because someone's already written a thousand lines of C behind the scenes for you. Okay.
[48:27] Oh, it really is pretty behind it. That's fine.
[48:33] Sorry. That was...
[48:35] Getting distracted on how pretty it actually is. That's fine.
[48:38] So I'm just thinking if I download something, so this came from a, maybe, I don't want a background, and I want block, please.
[48:53] So let's say I downloaded, what am I going to, Spotify, we're going to say Spotify, because that's where my mind's going right now.
[49:04] So it downloads, and this is a network access, blah, blah, blah. And then it downloads, and we go to having another box.
[49:19] Sure, we can have a black box, that's fine. And so when it gets to the box, it is sent to the CPU, which, give me a second to see
[49:33] if it goes to the right mindset, but then it goes to an interpreter, which then moves it to a, and then it runs the program?
[49:58] So the interpreter basically is another piece of code, which runs other code. It effectively says, I follow instructions you've given me, written in a different language.
[50:09] So this is where you do, like, JavaScript? Yeah, JavaScript, Java, Python, Ruby, C#, in most cases, all this stuff gets...
[50:26] Goes through the interpreter, and then... And that drives the CPU to do things, like, I say...
[50:33] It goes to the CPU to tell it to go to the interpreter, and then goes back to the CPU? So no, it's basically, the interpreter is a special program that just executes what
[50:45] it tells it to do, but it's on the CPU itself. So as I say, yes, for now, it's basically an alternate, like, if you imagine your operating
[50:52] system runs the C, the C code is basically telling your operating system to do things, the interpreter is that piece of C code, and your JavaScript's telling that bit to do.
[51:00] It's like an extra layer, rather than, like, you're wrapping things up. Okay.
[51:05] Okay. I feel like I can pause on this one, because it's at least giving me some idea of how to
[51:14] start conceptualizing it, because trying to figure out how data works is very complicated, I have come to realize.
[51:25] Yes. The problem here is that, like, in a lot of ways, what we do these days is quite far
[51:30] removed from the PDP-11 model I mentioned earlier, which is how a lot of people think about programming, and was taught programming, because we're old.
[51:40] And where this gets interesting is, like, if this stuff is, when you take it from the other side, and you build it up incrementally, you end up with a kind of more complete picture
[51:51] of everything, however, it takes a very long time, right? As in, there's just tons of, frankly, useless information in my head now, the systems that
[51:59] no longer exist, and for ways of programming that are no longer relevant. But they help me learn, and so many other things.
[52:07] They are quite good fun. But I will say, now that I have completely derailed us, and we didn't end up going to
[52:14] Spice Girls this time, I'm not sure where to go from here. Well, the logical answer is definitely to a rival girl band of some description.
[52:26] Okay. No.
[52:28] I honestly think, oh, gosh, All Saints was around at the same time, weren't they? I don't know.
[52:35] Problem is, this is where the problem with Spice Girls is, Spice Girls is international enough that everyone knows the Spice Girls, by comparison to almost every other band I
[52:43] can remember from the Britpop era. Well, I mean, you mentioned NSYNC last time, so we can go with NSYNC this time.
[52:50] NSYNC will do nicely. Right.
[52:52] Let's talk about NSYNC. And for this one, I am going to, do you want to share your screen, since I know that you're
[52:59] going to end up showing us stuff, or do you want me to continue and just scroll to wherever you need me to go?
[53:04] It's probably best if you keep scrolling, mostly because my screen is doing something strange right now, and I forgot to turn off Slack, and people are messaging me about things
[53:13] which are neither important right now, but things I can't, I want to make sure I have an idea of how to reply later, as is the case of everything.
[53:23] Also I have too many tabs open, my computer is running a bit slowly. Okay, cool.
[53:28] So the key thing, if we scroll back to, if you jump to where my mouse is, so there's a little button in the top corner where it says, like, just the B, and I just hit the
[53:37] B. Yay.
[53:39] Okay. So if we start at this point again.
[53:42] So now what we're going to talk about is, like, we're going to deal with the NSYNC discography, and we're going to deal with the fact that the data is now too, we're trying to deal
[53:51] with data which just keeps growing. So we're actually, you know, we're now Spotify, we have NSYNC, the NSYNC discography is a
[53:58] very popular piece of music, right? That's actually not that large, the total file.
[54:03] You know, you've ripped a CD years ago, a few hundred megabytes. So that's not too bad.
[54:08] You could feasibly have that on your machine for a single CD. But when you have, let's say, a band which is very prolific and has literally 30 albums,
[54:15] it starts to get a bit large. Queen!
[54:18] Queen, yeah. My gosh, Queen have a lot of albums.
[54:21] But then what happens is you think about how big is your playlist, your default "I like this" playlist.
[54:26] Right? 2,000 songs?
[54:28] Yeah, probably. 2,000 songs.
[54:30] And that's where it gets a bit difficult, because it's a bit too big, but these are all one, but these are all the same, so they're not too bad to store.
[54:39] So you just stream them as you need them and you cache the ones locally. But now you're net, but now you're actually Spotify, and Spotify behind the scenes has
[54:46] a record of everyone who's played any individual song, because that's important, because that's how they pay their artists.
[54:52] So they need to know that Jen played "Bye Bye Bye" 400 times last week. Right?
[54:59] Wow. Yeah.
[55:01] Yes. And they need to know that, and they need to know that Ben actually likes the Backstreet
[55:05] Boys slightly more. Shock horror.
[55:07] I know. Oh my goodness.
[55:09] I know. Right?
[55:11] And so this is where, like, these kind of numbers are really important, because that's how they pay the artists and deal with licensing things.
[55:20] So what happens is over time, the data of who did what and when grows bigger than the songs themselves.
[55:25] Right? Okay.
[55:27] So let's say they have, like, let's say they have, you know, a petabyte of music, right? Which is a lot of music, and potentially they probably have more, but let's say a petabyte
[55:36] of music. They can store that on some, they probably store that in multiple locations, so lots
[55:40] of people can read it at the same time, so it can be nearby people, and also read lots of times.
[55:45] But they probably have one or two very, very large databases, which have replicates of all the data of who played what, because I listen to Spotify, you know, probably close
[55:56] to 10 hours a week. Yeah.
[55:59] And most people I know probably use something similar. So every single one of those clicks is another hit on their database, so their database is
[56:07] probably tens of petabytes by now of their playlist of things. So that's way too big to fit on any single machine by a very, very large way.
[56:15] So what happens now is you think, I need to access all that data, right? I need to have, and the point is, really, is all that play data, you very rarely need
[56:23] to know who played a song at what point in time exactly once. So this is where we get back to access patterns, because I only care about play data in aggregate.
[56:32] I only care that you played XYZ number of songs, or how many times was Bye Bye Bye played by people, or by people in America, or by people in New South Wales in Australia, that
[56:47] kind of stuff, right? I care about, you know, a few small things with a smooth, small piece of detail.
[56:54] So this is all going to be loaded up the network, so you only care about moving what you should. So if we scroll to where I am, which is up and to the right, to this Column vs Rows data,
[57:03] right? So this is where we have all that columns data about all the plays, and this is why
[57:07] we use column stores, is we only care about one or two of these columns at a time, like all the plays, please, for, I don't know, give me all the plays by Jen.
[57:17] So I'm going to filter on the first column, which is who played it, and then on the third column, which is what they actually played.
[57:23] So I now have all of your plays at any time, so you can now scroll back through what you played when and where.
[57:29] Now I want to do a thing that says, give me all NSync plays, so the second column is the band, and so every single line is a play, so all I do is say, search where column A
[57:42] equals NSync, pull them all out, and I pull out all the durations, which is another column, so I only pull these two columns at a time, and now I have the total duration that NSync
[57:50] gets paid for. So this is why we store data differently, because the access matters.
[57:57] If I store this in Postgres, where everything's a row, right? Every time I pulled out data, I get the whole row every time I accessed it.
[58:07] Because we have the useless data at the end that says the metadata, like where you were when you played that song, which I don't need most of the time, or which device it was on.
[58:17] Very useful to some people who are optimizing for playing on phones versus Alexa devices, but not very useful for just how much we have to pay NSync.
[58:26] And if you imagine that these rows, there are, let's say, 400 rows, 400 columns, sorry, right?
[58:33] Going sideways, there might be hundreds of columns. If you imagine I had to pull hundreds of columns rather than the one column I actually needed,
[58:41] I am wasting time. So that is making sense.
[58:50] Would you say that it's easier to sort with column-type database? Yes.
[58:57] So the reason to use column databases. So it's filtering through.
[59:04] So column databases are optimized for the simple fact of, if you need aggregates where one column is deciding what you do in some way, it is nearly always much, much faster,
[59:16] potentially multiple hundreds of times faster to go through a column than it is to go through a row store for this stuff.
[59:24] Right? Okay.
[59:26] But also, caching tends not to work very well on these, because on average, what I want to know about the NSync plays, and what you want to know about, let's say, what mobile
[59:34] device someone's playing on, are two entirely different queries. So you don't really cache column databases very often.
[59:40] Okay. So, if you flip it around to instead say, I want to store playlists for Spotify, right?
[59:49] So I need to store them somewhere. They'll probably be in a database somewhere.
[59:51] They might even be in a, probably, probably in something like a MongoDB type storage solution. Right?
[59:57] Now, this is where caching is good, because they know that Ben loves to play his morning playlist every morning.
[60:04] Right? And I only really play from, I only really use two or three of my playlists all the time.
[60:09] So the cache they'll probably use for me, basically, only has those two or three playlists in it, and they know to retrieve them very quickly.
[60:18] They also know that, you know, that the playlist being shared by a big social media influencer is very likely to be hit lots of times, so they'll store that in something hot, cache,
[60:30] some hot cache. So that will be cached somewhere in RAM, rather than on a disk, because they don't want to
[60:35] read the disk every time to get that thing that's going to be read literally 100,000 times a day.
[60:42] Right. The example isn't really holding up at this point, but it's, hopefully, the kind of gist
[60:48] is getting across, which is that you store stuff where it's relevant. So, if it's a small piece of data accessed every time, like regularly, you'll keep it
[60:55] in RAM somewhere. If it's a random aggregation where it'll change quite differently every time, like, I don't
[61:01] need to know the same thing in every analytics query I do, you need to have a setup where you can actually just access all this stuff, and then just slice and dice through the data
[61:14] quickly. And that's making sense.
[61:19] I feel like I'm, my mind is going, what's out of this area? Like, oh, this is making more sense of why a playlist that I play often, if I'm driving
[61:31] somewhere and I lose service, it will still play, even if I don't have it downloaded, where-
[61:37] Yes, because it knows, exactly. So it has an intelligent on-disk cache, by the way.
[61:42] So Spotify actually stores quite more songs on your phone than you might think, because what it says is, it knows you happen to love that particular album by that particular band,
[61:53] and you play those songs all the time. So it'll intelligently say, "I'm going to store these here for now," and every time
[61:58] you play them, it resets the timer before it deletes it. Okay.
[62:03] And that's totally making sense. So let's say it says, "I need an intelligent cache of the top 100 songs Jen plays," right?
[62:14] But if Jen doesn't play a song for 30 days, for 10 days, let's say, I'll throw it away and replace it with the next most popular song.
[62:24] So then what happens is, if you do play, let's say, top 20 songs over and over again, they're always on your device.
[62:29] You can always play them, right? They'll always just play immediately next when you hit hot to them.
[62:34] There's no loading time, right? But now you want to add one of those brand new songs you've never played before.
[62:39] It takes a second or two to Spotify to link up. You'll notice it if the Wi-Fi drops out, but then you go back to an old favorite next and
[62:47] it's immediate, even when the Wi-Fi drops out. Yes.
[62:51] Yes. And that makes sense.
[62:53] Yeah. And this is like smart caching.
[62:55] So this is... And once again, it's caching because if you're storing an arbitrary number of things, but
[62:58] nearer to where you need them. Okay.
[63:06] That's making sense. I'm also over here writing down that someday we're going to definitely need someone on
[63:14] the show to talk about all the caching in the world and what is caching and what are they used for.
[63:20] So this is an interesting one because there's a famous phrase about programming and then a joke on top of that, which is there are only two hard problems in software engineering,
[63:32] naming things and cache invalidation. Naming things is always a problem.
[63:36] And then the other one is caching, basically, that is considered the second hardest problem in programming.
[63:42] Yes. Yes.
[63:44] And I'm not actually joking. Caching is genuinely one of those areas of actual hard engineering, though it is yet
[63:54] another one of those ones where, like naming things, you can get away with being pretty okay at it for a very, very long time.
[64:04] And I feel like now knowing that there's different types of caching is also making a lot more sense with all of this because I kept thinking of caching like browser caching, but being
[64:19] able to break it down to why browser cache is different and why browser cache may disappear, this is all like making so much more sense.
[64:30] This area by itself, I'm like, okay, cool. So it's all the same.
[64:38] That's my favorite line of everything is eventually the same, which is it's like fundamentally, like you're accessing stuff in your browser and it's caching it locally.
[64:44] So you don't have to go over the network to go get it, right? Same way as your video is buffered in RAM, so it doesn't have to go back to your SSD
[64:51] to read it. And it's exactly the same principle applies all the way down to your songs on Spotify,
[64:56] to the way you use Redis in front of a database, to why your CDs used to skip when you used to hit them.
[65:06] I feel like I have more questions about this yet at the same time, it kind of needs to sink in because I'm finally starting to understand the data side of it.
[65:19] Yes. Yet, I think something that would be cool for us to talk about sometime would be like,
[65:27] how is data created? Like I almost want to find you or someone else to come on and be like, let's talk about
[65:35] the history of data. Dan Moore has an amazing talk on the history of security.
[65:43] And he talks about how at one point there were two tribes on each side of the river and one tribe realized that they call the river, it's the same name, but one says it
[65:57] differently than the other. So they knew that there were imposters when they said the river wrong.
[66:03] Yes. That is a very simplified version, but knowing that had my interest way more into data or
[66:12] into security because I'm like, oh, that's how we actually got there. Yeah.
[66:17] So data and data storage and data access patents goes back a very, very long way away as well. So you think about things like the Dewey decimal system of libraries, right?
[66:29] That is an early example of an index, a perfect index symbol, a way of sorting data and indexing data for rapid access, because you don't know where the book is, but you'd happen to know
[66:39] already that the book is of a certain type. So you know you want to look at botany, so you know the code for botany, you can go to
[66:45] that section very quickly. So it gets you to the right place to start looking.
[66:51] And as you go back in time from there, you find like that's actually quite a sophisticated system.
[66:57] Earlier ones, you know, things like author name, very straightforward, understand? Your genre, your library is often another thing.
[67:04] But if you go back into things like recordkeeping and then things like the thing is in, I think it's, I can't remember which area of Italy the double entry accounting started, right?
[67:16] Because this is the idea of you map payments in to a payment out or payment out to a payment in every time so that you could add up both sides of the columns and if they went to zero,
[67:26] you knew you hadn't missed a payment. So this is why data was often stored twice in accounting, this is why data was stored
[67:33] twice in accounting. So this is about 600 years old now.
[67:37] So we're going back a few hundred years again, and this is like data storage, it was these were in books because these things had to be then transported by secure couriers between
[67:45] places so that if you borrowed money from somewhere or put money in one place from one place, you have to go back from the other place.
[67:51] So basically the book was the ledger that said, actually, we can give the king of France money today because we know he deposited money when he was in Paris and we can pull it out
[68:02] when he's in Naples. And that was done by a courier, transferring the data to know that the money was allowed
[68:08] to be shared. Interesting.
[68:10] And my favorite thing here is back to the security thing is it was done by people who are very not, they're very carefully known handwriting.
[68:20] Interesting. Yeah, there's so many different types of security that I, I found his talk so interesting that
[68:30] I had no idea that much went into it and to be able to talk about it now. Security is such a huge field.
[68:39] It's ridiculous. It goes back.
[68:41] It's one of those, it's also a truly old field, like, so data is a very old field as well, but in a lot of ways it's, it's sophistication.
[68:52] How sophisticated it is goes up and down over time. Like there are times when no one cared, particularly like, like there are cultures where you are
[69:01] in, where your birthday doesn't matter because you're born in the season. Oh.
[69:07] And that's the precision, the level of precision they'll work to, right? There are other things where like, things where the exact number of things you own isn't
[69:19] important for various reasons, or things that collectively own, therefore ownership is not direct.
[69:24] Some things are collectively owned. Therefore no one would have knowledge of exactly how many things there were because everybody
[69:29] might have them. Who knows where they are, right?
[69:32] And then we get to think, it's when you get to places where like, where you, particularly like, if you look into things like the ancient Egyptians had a lot of data storage in like
[69:43] tablets and things, so that they could have a more complex economy, but their economy was still, still barter-based.
[69:48] When we get to money, money then accelerates this data boom, and the Romans had great detailed things.
[69:55] They still left the concept of zero though, so owing people money was very strange. I feel like you just, you/Dan, gave me a great talk idea.
[70:07] Now I want to go research of how data became data. I would love to hear that done because it's one of those areas where I have a lot of bits
[70:17] of knowledge and no through line through any of it. It's fascinating.
[70:21] The double entry accounting thing is fascinating because of, so I met a guy called Jerome Grief recently at a conference I was at.
[70:28] I've been following him for a while. He's building a database called Tiger Beetle, which is open source and written in a language
[70:33] called Zig, which I'm a fan of, and it is a database specializing in accounting, and double entry accounting is a fundamental principle in the database.
[70:45] Because if you think about it, most accounting systems are just done on top of databases built for other things, and this one's actually like double entry accounting is literally
[70:54] a core piece of the system, which gets two interesting things. The first is you get double rights, therefore you actually have more data protection than
[71:01] you might think, but also it automatically keeps storage in the way that accounting rules require as a file format effectively, which is quite special.
[71:12] Interesting. So much.
[71:14] I'll see if I can get him to do one of these with you, actually. He'd be an excellent guest.
[71:20] Yay, that would be amazing. Yes.
[71:22] He gave an absolutely amazing talk on how data is stored recently at the event QCon where I was at, and it was amazing.
[71:31] I was making furious notes and tweeting along, because it turns out there's a lot more things going.
[71:39] You actually have to start writing data to disk, and when you write to disk, and how it's written to disk.
[71:43] These things, because we've gotten so far along the journey from the older computers designed in the '80s, the abstraction level we've got to, even just in our operating systems,
[71:53] is so high that things aren't as easy as you think. Until relatively recently, Postgres wasn't as secure at writing data to disk as people
[72:01] thought it was. What is his name?
[72:04] Do you remember? I can find it for you, Joran Dries, but it's one where my ability to pronounce versus spelling
[72:12] is never straightforward. I was just going to say, can you link the video?
[72:17] If the video is out yet? >> It's behind a paywall.
[72:19] >> Just kidding. I mean, let's link it anyway, because if others want to pay to view it, we should probably
[72:28] link it. >> I'll show you his Twitter profile.
[72:31] >> Perfect. >> I'll just ping you on our Slack for now, and we can go from there.
[72:37] I'll ping you on my, I'll intro you on Twitter. >> Yay.
[72:42] Perfect. Well, then I, oh, hey, we follow each other.
[72:49] >> It's a small world. >> It is.
[72:51] It really is. I always get really excited when, this happens a lot, when I'm like, I follow them.
[73:00] They follow me. This is fun.
[73:02] When I had no idea what they do and all that. >> So we took a picture together at QCon, and then a mutual friend of ours reached out
[73:08] immediately to both of us, like, hey, you know so-and-so? >> Yes.
[73:12] Yes, that happened yesterday, because Dan Moore was on my friend Ramon's and Rizal's show where they do CFPs and talk practice.
[73:25] And so I was like, wait, y'all know each other? Huh.
[73:30] I did not realize that. And it's so fascinating.
[73:35] It's such a big and small world all at once. >> There it is.
[73:40] >> Yay. Cool.
[73:42] Well, I will say that I'm probably a little -- I don't want to say fragile. My brain is starting to be full.
[73:53] So I have a lot to work on. I can say that.
[73:56] And there's a lot more -- >> You've entered disk swapping mode. >> Yes.
[74:01] I need to disk swap. >> So that's actually a thing where you run out of RAM, and you need to swap -- what's
[74:07] known as swap disking is where your RAM swaps in and out of your hard drive. So you're storing things on the hard drive because you're out of RAM.
[74:13] >> Oh. So you move it from the RAM to the hard drive so the RAM can erase itself.
[74:18] >> Yeah. And be reused.
[74:20] Because it is not being used right now. So if you ever run into a swap disk thing on Windows, that's what it's talking about.
[74:28] >> This is a very silly way of -- it's not Windows. It's on Genshin Impact.
[74:32] It says the CD is switching. >> Like that, yes.
[74:37] So when you run out -- so the funny thing is, there's a really, really good video I will share, and I recommend you share it to the crowd, which is talking about the original
[74:47] Crash Bandicoot game. Right?
[74:49] >> Oh, I love Crash Bandicoot! >> Because of disk streaming and all the tech that does all that stuff and live caching
[74:55] of disks was invented by the Crash Bandicoot team, in most cases. Because of -- do you remember how much better Crash Bandicoot looked than every other PlayStation
[75:04] 1 game? >> Yeah.
[75:06] >> For the longest time? >> It looked pretty much better.
[75:08] Right? >> Okay.
[75:10] This is -- do you remember an IQ cube game on PlayStation? >> No.
[75:15] >> There was, like, a cube game where you were a little human and you had to guess what cubes were going to fall towards you.
[75:24] >> So I didn't have a console in PlayStation era. This was back -- so I went in and out as a PC gamer.
[75:32] So I used to have a Famicom in the -- in the SNES era, I had a Famicom, an actual Famicom, because we lived in Pakistan for a brief period of time, and it was what we could find.
[75:46] And then later, when it came around to the PlayStation era, we were mostly PC gamers, and we got a PlayStation way deep into the middle of the PS2 era, because it was secondhand.
[75:57] And that's the classic thing of, we wanted to play Final Fantasy, me and my brother. So we played Final Fantasy VIII so much.
[76:07] >> That makes sense, and I -- IQ cube, I used to try to Google it, and I could never find it, but either my Googles have gotten better, or Google is starting to learn what I actually
[76:19] mean instead of what I'm typing, which I think is that, because, well, but I found it. Oh, my gosh.
[76:28] >> Oh, wonderful. >> I don't know if it's available anywhere, but I am -- I will share my screen briefly,
[76:35] because look at it. I'm so excited.
[76:39] Let's see. It's this game.
[76:41] I don't know why it was so entertaining to me. I would play this stupid game for hours.
[76:51] >> So I didn't know this was the original, because I've seen so many people trying to recreate things like this in so many of the gaming, like, forums, subreddits I'm on.
[77:01] I did not realize there was a PlayStation game they're trying to imitate. >> This game, like, I love this game.
[77:10] This game is everything. And I should actually see if there's a way to play it now, because I -- well, no, I'm
[77:20] going to say I probably shouldn't, because I will waste way too much time playing that. >> So the video I've linked to you, and I recommend sharing, because this is a genuinely
[77:29] brilliant one, is about memory constraints and disk constraints on the PlayStation. >> Yay.
[77:35] >> To the point where they filed patents for the technology they found. >> That's so cool.
[77:40] Okay, I'm linking that to -- >> Because it was so short, and, like, so loads of PlayStation games had very small levels by comparison to Crash, because Crash
[77:48] could stream levels, whereas they couldn't, which is why Crash Bandicoot looked better than every PlayStation game for, like, the first three years of PlayStation.
[77:59] It was, like, the best-looking game by a really long way. It was still good-looking, even by the end of the era.
[78:06] >> Yeah. But Crash Bandicoot and Spyro, I don't think that they were made by the same people.
[78:12] >> I don't. >> Spyro.
[78:14] >> Spyro holds a special place in my heart. >> Because Spyro had pretty good graphics, too.
[78:20] >> Yes. >> And I think it was around the same timeframe.
[78:24] >> It was. So I don't -- by the way, this is, like, early Naughty Dog as well, so the people who made
[78:28] Last of Us, eventually, were the people who made Crash. >> Okay, so Crash Bandicoot came out in -- now it's not telling me.
[78:43] >> 1995, I think? >> History, 1996.
[78:49] And Spyro first released in 1998. So, yes, around the same timeframe, but I wonder if the technology went to more programs
[78:59] within those two years. >> It probably did by that point.
[79:04] So yeah, so they were by Insomniac. Insomniac were another, like, pioneering studio, anyway, so they might have had some of the
[79:09] same people, to be honest. >> Yeah.
[79:11] It was definitely -- I still have it. I downloaded it for my Xbox, they have it, and I'll play it for a while.
[79:20] It's definitely -- I was always more into those, except Mario 3 and Mario 2. >> Okay.
[79:28] >> Because those were also my go-tos. >> So I definitely played Spyro quite a bit.
[79:35] I was always more of a PC -- because I played PC games mostly, so I was stuck into Command and Conquer Land for a very long time, and things like Shogun Total War, and equivalent
[79:46] like that. And I've mostly played a lot of RTSs.
[79:49] >> Yeah, a few of the D&D crew that I'm a part of, they want to start playing, like, what is it called, SC2, StarCraft 2?
[80:02] There we go. >> StarCraft 2, yes, I still play it.
[80:04] >> And I'm like, strategy games, IQ thing, I'll play it all day. Strategy games, I'm like, no.
[80:14] So first-person shooters. >> So, genuinely, I don't play those anymore, my eyesight's too bad these days, but I play
[80:20] a lot of strategy games. I actually got a job once by playing Age of Empires with the company founder, pretty much.
[80:27] >> Oh, wow. >> So, okay.
[80:29] So, oddly, this does come to another data question, so this is fun. So back in the day, like the 2000s, that's not even back in the day, having computer
[80:47] cafes. Like, you would have to bring your own computer a lot of times to go play a game against your
[80:54] friends on the same LAN internet? >> Yep, same LAN, yeah, local area network.
[81:02] >> Okay. So, it would still be, like, an external or a network access?
[81:08] >> So, not really. So you all, so LAN gaming comes from the era of you all had the same game, you all installed
[81:17] on your own machines, right? Every single machine had a copy of the game, right?
[81:21] So, how game networking works is worthy of the whole chat on its own. I have a talk out about this, actually.
[81:31] I gloss over the details to explain it in relation to other things, but the key thing really is that fundamentally you don't send, like, you don't need to send, you don't stream
[81:41] the whole game from one person to another person very often. Normally what happens is you and I have the same game running on our machines with all
[81:48] the same data in it. What happens is if I say, "Move left," I send you, Ben's character moves left.
[81:54] >> Okay. >> And on your machine, you go, "Acknowledged."
[81:59] And Jen's character picked up a brick, "Acknowledged," sort of thing. And what happens is, behind the scenes, our game, the game software running on each of
[82:09] our machines, synchronizes its state between each other, dependent on exactly how the game is being networked.
[82:15] That's normally what happens. One person is the authoritative leader of the game, or one machine is, and effectively
[82:22] all updates of the game are agreed by that machine, and they're streamed out to everybody else.
[82:26] And we just share the tiny changes. >> Okay.
[82:29] >> So we can change it, so we can share them as fast as possible. >> Okay.
[82:35] >> So, an example of how it can take a while is, if you've played Minecraft and you've joined a new world you've never been to before, and people have done a lot of edits, it takes
[82:45] ages to load up the map, right? That is when it's streaming all those bits over the wire.
[82:51] >> Okay. >> Or VRChat does this as well, when you go to a new place and you have to load up the
[82:56] whole new room, and it's big, it takes ages for it to stream it. >> I'm also listening while trying to draw a computer that's not going very well, because
[83:12] that's a very useful part of it, to draw land, which, okay, this does make sense of why you would have a primary computer as well.
[83:21] >> Yes. >> So, a lot of things to look into, and I will also add that to my notes of ideas.
[83:31] >> Game networking used to be my job for a long time as well, so, like, it's one of those things where it's like, it is a deep, it is one of those areas which starts off in a deceptively
[83:41] straightforward place, but rapidly becomes about dealing with the eccentricities of how weird people are, and how weird, like, how weird the computers are, and effectively faking
[83:53] everything you can get away with. >> So, I think this is just decided, you will just be on the show every so often for forever.
[84:01] >> Thanks, Ben, now we have two Bens on the show often, this is going to be fantastic, yay, because Ben Myers talks about accessibility a lot, and it's fantastic, I should send you
[84:15] some of their content, I think you would really like it, if you don't follow each other on Twitter, you should, but, yay, okay, well, this will wrap up for this week, and I know
[84:28] with my progression with Postgres and all the databases, I will have questions by next time, I just, at the moment, I'm switching disks, is that what it's called?
[84:42] >> It'll do, you'll swap it, you'll activate, swap disk, so, yeah, you're moving memory from RAM to disk, so you can do other things for a bit.
[84:54] >> It's like sleep. >> Yeah, so, this is what hibernate is, when you hibernate a laptop, it literally saves
[85:02] all the RAM to your disk, and then loads it all back again when it wakes up. >> But it's like human sleep.
[85:10] >> Human sleep is really weird, like, the more I read about sleep, the more I'm like, this makes no sense.
[85:17] >> Interesting, well, on that note, thank you, everyone, for joining today, and please put down in the comments what questions you have, you can follow both of us on the Twitters
[85:28] as well as find us on LinkedIn, Mastodon, I'm on Mastodon, are you on Mastodon? >> I am, I'm on Hackaderm, I'm @bengamel7.
[85:37] >> Me too, me too, but Jen, not, yeah. >> Same handle.
[85:43] >> Yeah, same handle on both, because I am incredibly lazy when it comes to handles. >> Yes, and thank you, everyone, and bye.
[85:52] you 
