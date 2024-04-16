---
showLink: "https://www.youtube.com/watch?v=ZfLAxjAP8fI"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-hosting-with-roy-anger"
title: "Teach Jenn Hosting with Roy Anger"
publishDate: "2023-04-18"
coverImage: "https://i.ytimg.com/vi/ZfLAxjAP8fI/maxresdefault.jpg"
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

[00:00] to another episode of Teach Gen Tech. And today we have Roy coming on the show.
[00:06] And I can tell you, this is because I thought something finally clicked
[00:13] and it really didn't. And luckily Roy offered to come hang out.
[00:18] And before I have Roy talk about everything that we're doing I do wanna say that I met Roy
[00:25] from being part of the Open Source Raid Guild. As y'all know that I talk about D&D enough.
[00:31] And that Roy has our new, what did we call you? Did you say game manager?
[00:38] - Yeah, I mean, you can call it Dungeon Master too but usually if there's not dungeons
[00:41] it's people call it Game Master. - Like GM makes me think of like general manager.
[00:46] - Well, I mean, that's what they are, right? Dungeon Master is the general manager
[00:50] keeping everyone in line and like setting the rules and making sure everyone does their job.
[00:56] - This is true, this is true. And we just started, we're starting a new game
[01:01] when I get back to town streaming more regularly called The Expanse.
[01:07] And if nobody has watched the show, it's really cool and come watch us stream on Sundays.
[01:12] But that's all for another day. Roy, who are you and what are we gonna be learning about?
[01:19] - Yeah, so obviously my name's Roy. I work in full stack development.
[01:24] I do React, usually React on the front end. I've been doing solid, I even have my solid mug
[01:30] if anyone from the solid team is around and cheering on. And on the back end I usually do Node,
[01:36] I've been learning Go as well. Yeah, so just build web apps with those languages
[01:43] and like the related technology. And as Jen said, I'm a big fan of The Expanse
[01:49] and running The Expanse campaign. Not only if you haven't watched the show,
[01:53] I'd also say if you haven't read the books, the books are excellent
[01:55] and they contain even more story than the shows. There's like another three seasons kind of deal.
[02:03] So lots and lots of stuff. - I'm excited about reading the books
[02:08] once I'm done with the show, because I feel like if I am doing both,
[02:12] I'll get confused which one is which. Like the storylines will overlap too much.
[02:18] - Yeah, for sure, I definitely recommend that. - So I'm very much looking forward to,
[02:24] soon I will be reading those instead. - Yes, and what are we talking about today?
[02:32] - Well, we're gonna hopefully answer a bunch of your questions about hosting and how it works
[02:38] and what the differences are and maybe give some information to you and your listeners
[02:43] about what to choose depending on what the projects are. - Ooh, yay.
[02:48] And y'all, I am linking in the, link to the tweet, to the Twitter,
[02:56] to the tweet about what I thought was accurate, but it's definitely not,
[03:01] because I used to work at GoDaddy. And when I worked at GoDaddy,
[03:08] it was like, there was regular, what I called regular hosting,
[03:13] 'cause you know, people would call in and be like, "Yo, I need to put my website somewhere."
[03:18] And we would say, "Cool, "do you want to be able to customize it and do things?"
[03:24] And they're like, "No, I know nothing about it. "I just wanna be able to have a website."
[03:28] We'd be like, "Great, here is a website builder, "like Squarespace or Wix or something like that."
[03:36] And then after that, it was, if they wanted a little more customization,
[03:42] it was like managed WordPress. And you know, managed WordPress could do a bit more FTP,
[03:49] but not like a ton more, there was a bit more customization.
[03:54] Or if they wanted all of this really cool stuff, they could go to cPanel Hosting, which was shared hosting.
[04:03] And so, that's my hosting knowledge. And then there's Vercel and Netlify.
[04:09] And I'm just like, wait, what? You also technically host and it's free.
[04:15] And I get an SSL, what? And this is where I got very confused.
[04:21] How does this work? - Yeah, and there's a lot to all of that.
[04:26] So, let's start with WordPress and let's start with, or not even WordPress, sorry, let's start with GoDaddy.
[04:31] And let's start with kind of defining what a webpage is at the basic level,
[04:37] 'cause we're gonna be kind of like expanding on that as we go.
[04:41] So, I guess, quick question for you, Jen, what is the minimum thing you need
[04:46] to have an actual webpage? - Minimum thing?
[04:53] Yeah, FileZilla. - It's coming, yeah. - Yeah, FileZilla is all you need.
[05:00] Yes, and I've talked to many people through FileZilla and SFTP and that kind of thing.
[05:08] I almost wanna say HTML. - You got it.
[05:13] You need an HTML file. - Okay, good. I was like, do you need a domain?
[05:18] And I was like, no, I don't think you technically need a domain, but--
[05:21] - No, you can do it via an IP address, but that's the hosting side, domain and the host.
[05:27] But an actual webpage is just an HTML, like at the core is an HTML file.
[05:32] Everything else is adding on to that, right? So, you have CSS to make it look better,
[05:37] images that will provide visual content, or in some cases, background images to make it look better.
[05:42] And then we add in other stuff like JavaScript on the client side or potentially the server side,
[05:50] and then stuff like PHP, Ruby, Python on the server side to allow us to have dynamic content
[05:58] of different types and different looks. So, if we think about that with WordPress,
[06:06] WordPress is basically, well, it's not basically, it's all written in PHP.
[06:12] - I don't think I ever knew that. - That's all written in PHP?
[06:17] - Yeah. - I mean, the role that you were at at WordPress,
[06:21] yeah, it was probably one of those things where the people who knew it
[06:25] thought it was so obvious they wouldn't say it, and you didn't really need to know it.
[06:29] So, you just kind of, you could do your job without really knowing it.
[06:32] And it was so obvious to people who knew that they didn't bother saying it.
[06:37] - And it's so crazy because like, and for more context of where I think
[06:43] there's so much confusion in this, I also helped with GoDaddy hosting WordCamps
[06:50] and doing WordPress-y things. So, I kept seeing the consumer side of it,
[06:57] not what happened to build it, which going into software development and coding itself
[07:05] is much more on the infrastructure side of what goes into building it.
[07:10] And that is a great call out on why I'm lost of, I didn't even know it was PHP.
[07:16] That's cool. - Yeah, no, that's all good.
[07:19] Yeah, so it's written in PHP. PHP, like Python, like Ruby, and other languages,
[07:25] every language with JavaScript is server-side rendered. So, what that means is,
[07:32] instead of having an index.html file that you can just send directly to the client
[07:36] and the browser can load it, you have an index.php file.
[07:40] If that gets sent directly to the browser, the browser's like, "I don't know what to do with this.
[07:44] "PHP, what's this stuff?" So, what happens is when you request that page,
[07:49] so like teachgentech.com or whatever, if that file on the server is an index.php file,
[07:58] the server will read it and it will have a module or support to execute the PHP code,
[08:06] do whatever the instructions are, connect to a database or load information from a file
[08:13] or connect to a third-party API and get information, whatever that is,
[08:17] and it'll execute all that and then it'll generate an HTML file
[08:21] and send the HTML file to the client. And then the client can display that.
[08:25] - Hi, Ramon. So, just to make sure,
[08:34] because I really should just share my screen when I'm doing this,
[08:37] so that way people actually know, A, why I'm just staring down awkwardly at my computer
[08:42] and then are at my... Hey, look, it says good daddy, yay.
[08:48] So, what you were saying is like PHP goes into like a module that renders it into HTML.
[08:57] Is that what I heard? - Yep, it's a module on the server.
[09:00] So, I guess, actually, let me even back up a little bit more.
[09:04] So, server is this generic term that can mean a lot of different things.
[09:10] There's server, like the hardware server, the actual computer that does stuff,
[09:16] but there can also be... That server is also used in the context
[09:19] of particular pieces of software. For example, you have a website server
[09:23] or you have an email server, et cetera, right? So, your hardware server that does web hosting
[09:33] will be running a web server software. When it comes to WordPress,
[09:41] traditionally, that was called Apache. Most places have moved over to something called Nginx.
[09:48] It doesn't really matter. But that software accepts requests,
[09:55] web-based requests. It looks at what file was requested,
[10:02] checks to see if that file is present on the server, and then will serve that file to the user.
[10:09] Now, serve depends on what exactly that file is. If it's an HTML file,
[10:15] serve will just be sending it to the user. If it's an image or a CSS file, same thing.
[10:19] It'll just send it to the user. If it's, in this case, a PHP file,
[10:23] that piece of web server software will first execute the PHP code and get the final result.
[10:31] And then that final result will be an HTML file and then send that HTML file to the user.
[10:38] - I think that's also something that may have been very, very clear when I worked at GoDaddy,
[10:44] but looking back at it. And y'all, for context,
[10:48] I worked at GoDaddy in the email department and the hosting department as sales and support
[10:53] and team leadership for about five years. And so like, it's just funny to me
[11:02] because you said email server. And I'm like, yeah, okay.
[11:04] And you said hardware server. And I'm like, okay, cool, totally get that.
[11:07] And then you said software server. And I'm like, wait, what?
[11:12] That's a thing? That's, wait, what?
[11:15] Because I think back in the day, even now, I always meant that hardware and software server
[11:21] were like the same. And this is a big reason why Ben said
[11:27] that he has an extra Raspberry Pi I can build. So when I see Ben Gamble next week,
[11:34] I'm gonna get that. And then when I get home sometime next month,
[11:38] I am gonna build it. So I understand hardware a little bit better.
[11:41] - I think the easy comparison here is you have a Mac. You're using a Mac right now, right?
[11:49] - Yeah. - So your Mac, you're using minimum three things right now.
[11:54] You're using the actual physical computer, which is the CPU, the hard drive, the RAM,
[12:00] the motherboard, et cetera, the display. That's the hardware.
[12:04] It's not a server because it's a computer, personal computer versus a server.
[12:11] Then you have the operating system, which is Mac OS. And then you're using at least a web browser
[12:19] for StreamYards and Twitch and stuff like that. You're probably using a bunch of other pieces of software,
[12:23] but you're using at least a web browser, right? So if you think of that,
[12:29] you have the actual physical computer, the operating system, and then the web browser.
[12:36] The comparison on the server side is you have the server hardware.
[12:39] That's just a big, powerful computer hooked up to a very powerful network.
[12:45] And then you have an operating system on servers. It's almost always Linux.
[12:50] Sometimes it's Windows, but it's mostly Linux. And then you have the piece of software that's being used.
[12:56] On your computer, it's the web browser. On the flip side, on the server,
[13:01] it's the HTML server, the web server, right? And then your browser and that web server
[13:10] are communicating back and forth. - I am also looking at something for comparison is,
[13:17] okay, yes, cPanel, which is what most of GoDaddy's content was using
[13:28] when they were accessing their shared hosting was cPanel as well.
[13:33] So that helps. Yes, it's still Linux.
[13:36] - Yep. - Okay. - So cPanel is essentially a tool
[13:42] that lets you access a bunch of different services on the servers on GoDaddy.
[13:51] So cPanel will let you access the FTP server to create or change FTP accounts.
[13:58] Watching you type and trying to say FTP. - Right.
[14:02] - It also let you create and change FTP accounts. It'll let you access the email server
[14:08] and add and change email accounts. It also provides you access to like an email client
[14:14] so you can read emails through the web now. It'll access at least the file browser
[14:21] as well as some other stuff for the web server so that you can see the files that you have for the website
[14:29] and make changes and upload files. It'll have access to your database,
[14:37] usually via phpMyAdmin, which is just a tool to manage your database remotely.
[14:42] So cPanel is just like an interface that brings a bunch of these management tools
[14:46] for all of those different software servers, right? The web server, the FTP server, the email server,
[14:52] the database, which is a server, your domain name server.
[14:57] So it lets you access and manage all of those from one place. - I'm just realizing like, as you're telling me this,
[15:10] I'm like, I don't think I realized how many types of servers there were.
[15:14] This was a big experience while streaming with Ben talking about how many different caching there is.
[15:26] Like there is like, you know, the computer caching, then you have your browser caching,
[15:31] then you have like, he mentioned like seven others and it's like, oh, okay.
[15:37] And I'm realizing it's the same way here. - Yep.
[15:44] - Okay, cool. So going back to the example you gave earlier of like,
[15:52] so WordPress is built with PHP, cool. Totally didn't realize that.
[15:57] Now, if somebody is taking that index.php, then it is the software server that is turning it into HTML.
[16:08] - Yep, the web server, right. Specifically. - The web server.
[16:14] - Okay. Yay, another server.
[16:19] I will do index.php and then it goes here and then it comes out as HTML.
[16:33] - Yay. - Assuming everything, all the code works
[16:36] and everything, of course. We'll just, for the sake of today's discussion,
[16:38] we'll assume that they're not, you know, breaking bugs and things failing all over the place.
[16:42] - Who knows, if I'm doing it, it probably will. - Happens all the time, everywhere.
[16:48] - Okay, and so could you give me another definition or way of explaining web server?
[17:00] So is web server basically everything up here except hardware?
[17:05] - No, it's none of those, it's like, it's its own one. - Yes.
[17:12] - Email, FTP, domain, database, web server, they're all software servers.
[17:17] - Okay. - Software server isn't really like a proper term.
[17:24] I'm more using it to kind of like. - Visualize, yeah.
[17:29] Like people don't usually call them software servers, at least not in my experience.
[17:33] - So and then we have our one lone hardware server. - I mean, yeah, like it's just physical hardware,
[17:45] exactly what it is and how it looks is different in all the different cases.
[17:48] - Okay, cool. I think I'm following at the moment.
[17:54] So WordPress is going to be shared by WordPress. - It's going to be shared hosting.
[18:01] - It doesn't have to be. - It doesn't have to be.
[18:03] - We're going to get into that, don't worry. - Okay.
[18:06] - So yeah, so talking about shared hosting. Companies like GoDaddy, there's Bluehost,
[18:15] there's SiteGround and dozens of others. And they all specialize in WordPress hosting.
[18:20] Most of them offer as their primary service shared hosting. So shared hosting is a very powerful server
[18:30] that handles thousands of sites. Now they make money on this
[18:37] by selling the hosting super cheap, but they also, the reason they call it shared
[18:44] is the resources, the CPU, the RAM, and to a lesser extent, typically the hard drive space
[18:50] is shared between all of the sites. These companies will,
[18:56] they will take and put more sites on the server than the server could handle
[19:08] if they were busy. They assume, and rightfully so,
[19:13] because most WordPress sites are not very busy. They're personal sites, they're small business sites
[19:20] that don't see a lot of traffic. They understand that a lot of these sites
[19:23] don't need a ton of resources to run regularly. So they pack a number of sites onto these servers
[19:32] so that they can maximize their profits. But therein lies the problem.
[19:38] They're assuming that these servers aren't that busy. In some cases, if a number of the websites get busy
[19:46] or one or two of the sites get really busy, it can impact other sites on the server.
[19:52] - Ooh, I remember that. - And let's just, what's the best way to word this?
[20:01] One of the companies that we have talked about today is notorious for being not great at this
[20:09] and having a lot of performance problems by putting too many clients on their shared hosting
[20:14] and causing a lot of performance issues. So different companies will handle that differently.
[20:26] Some will have more sites, some will have less sites. And so you'll see kind of a different quality
[20:34] in these companies depending on how they're setting up those resources.
[20:39] - That's not what I wanted to draw, but that's fine. So it sounds like it's kind of like airlines
[20:46] or movie theaters. They're gonna sell extra tickets
[20:49] than what they actually have seats for. - In Canada, we don't, well, maybe after the pandemic,
[20:55] I haven't been to the movie theater since, to be fair, but before the pandemic,
[20:59] we never oversold our movie theaters up here, but maybe it's a thing now.
[21:03] But definitely like airlines, yeah. And obviously like airlines, when everyone shows up
[21:11] and no one cancels last minute, you have a problem now. You have too many people for the plane
[21:16] and you've got to figure out what to do. If someone gets upset or you've got to pay someone
[21:19] or whatever. - I'm really hoping you guys can't hear my dog again
[21:37] 'cause she is on mute. - I like heard the slightest sound.
[21:43] (faintly speaking) I can't write.
[21:50] Should be shared. We'll go with that.
[21:59] How many are actually shared? - The problem with this is like
[22:06] when it comes to shared hosting, there's no, the only answer is like,
[22:12] the only answer that's 100% safe is, would be based on how many resources you're promising.
[22:18] But so that's where you move away from shared hosting and you move to other forms of hosting.
[22:24] Let's see what GoDaddy's offering these days. - I do not think that is how you spell guaranteed,
[22:34] but you know, we're gonna go with it. It is a word that I've never been great at spelling.
[22:42] Or maintenance. Anybody really good at spelling maintenance?
[22:45] 'Cause that is also not a good word for me. I don't know why.
[22:49] - Somehow I've spelt it a lot, so I'm comfortable with it, but no, I feel your pain with some of these words.
[22:55] Necessarily is one that I always have to like think about. So I'm just checking GoDaddy's offerings
[23:05] to see what they even have. - And if you want to share your screen, just let me know.
[23:12] I am honestly just-- - I'm just skimming through really quickly.
[23:16] - Trying to rewrite guaranteed. - Sure, that'll work for now.
[23:23] - Okay, so they have, looks like the only options they have
[23:39] that would move past shared hosting are the VPS hosting or their dedicated server hosting.
[23:47] I'll talk about it in a second. I'm gonna mention, when it comes to WordPress hosts,
[23:52] you're gonna see a lot of managed WordPress sites, and that's usually something that people pay more for.
[23:59] Managed WordPress hosting or managed WordPress sites basically means that
[24:08] the host company will update WordPress and plugins, which is generally really easy to do,
[24:15] and then they'll tend to add a basic free tier from a software company like Securi,
[24:23] and they'll do backups. And so that's what managed means.
[24:28] It's just some basic automated stuff. It's not a lot.
[24:31] It certainly isn't anything on the server level. It's no different.
[24:38] It's just some management of your site. - And thank you, is it Yarmulinko?
[24:46] When there's no spaces in people's names, I'm always guessing how to say it.
[24:54] Thank you for the follow. - It's always a guess.
[24:58] Is it meant to be part of their first name and last name, or is it completely made up, or like?
[25:02] - Yeah, I always feel bad because I'm totally always butchering people's names.
[25:07] So yes, I do remember that it was like automated updates if it's a managed WordPress.
[25:13] I'm pretty sure that they used to include SSLs in managed WordPress.
[25:19] - Oh, maybe, yeah, maybe. - I don't know.
[25:21] It wasn't like- - I don't think so, though. - That's why I always got so confused.
[25:26] - I know you do. At least right now you do.
[25:28] I don't feel like they used to, but I might be wrong. - Yeah, that's why I was like, I don't know.
[25:33] Wait, that's not SSL, SSL. I mean, that could be its own, like, stream.
[25:37] What's an SSL? Let's not go there.
[25:40] Let's, secure socket layer. It's what makes HTTP into HTTPS.
[25:46] Okay, anyway, that's that. So I believe you also said that there was a VPS
[25:51] and there was one other one, dedicated server. I'm just writing it.
[25:55] - Yep. - Cool. - Yep.
[25:57] So VPS is actually, VPS works kind of the same as shared hosting.
[26:06] The difference is, so VPS stands for virtual private server. So virtual private server, you take that,
[26:13] that big, powerful hardware server, and you slice it up into essentially like,
[26:18] think of like slicing it up into slices of pie. In the case of VPS, they can be different slices.
[26:25] One slice could be small and it has one virtual CPU core, you know,
[26:30] four gigs of RAM and like 50 gigabytes of SSD space. And then another one could be a little bit bigger
[26:39] and it's twice that, two virtual CPU cores, eight gigs of RAM, a hundred gigs of space.
[26:45] The key with this is that those, whatever your VPS service, like, settings are,
[26:54] those are yours. You pay for them and you have them.
[26:58] They're not shared with anyone, right? So if you are supposed to have four gigs of RAM,
[27:04] you'll have access to four gigs of RAM. So you don't have to worry about other sites
[27:09] affecting the performance of your site. The only reason you would run out of resources
[27:13] is that your site gets busier and you would need to upgrade your VPS
[27:17] to something more powerful. - And if I remember correctly,
[27:22] oh, thanks, Ryan. I am grateful that people do like my handwriting
[27:29] 'cause I'm like, I don't know what I would do if I couldn't be writing all of this out
[27:33] because I was like, it helps my brain so much. - I write stuff out, but no,
[27:38] I feel sorry for anyone who has to try to read my handwriting.
[27:43] It's the exact opposite of yours. - Really funny.
[27:47] If my mom ever caught one of these streams and saw my handwriting,
[27:49] she would still tell me I have horrible handwriting, but that's because I'd never properly learned cursive,
[27:55] but there's like words that you'll see that I write that are like half cursive, half like-
[28:01] - Yeah, I do that too. - Do they still teach cursive in school?
[28:06] Anybody know? - I have no clue.
[28:09] - I'm so curious. - I've been out of school for a very long time
[28:14] and I have no kids too who are learning, so couldn't tell you.
[28:17] Maybe someone in chat knows. - Yes, somebody in chat, please riddle us this
[28:22] because I am very, very curious. I'm moving this over because I feel like something
[28:29] that also needs to be added here, which I think is another part of the confusion.
[28:36] I didn't want to just default go to GoDaddy colors, so let's like use a different green,
[28:40] is when it's like a managed WordPress, it's definitely not as much to technical knowledge needed
[28:52] as like plugins and stuff like that from this is going off a memory.
[28:58] When going to a like a cPanel or shared hosting like that or like VPS is you need somebody
[29:10] that can manage the resources better. So when somebody called in for hosting
[29:20] and they set up like cPanel is what I'll call it, it was like GoDaddy and this is five plus years ago y'all,
[29:30] I don't know what they currently offer, is like their shared hosting would be like cool,
[29:37] if you're having some issues with the resources, we'll help you figure it out.
[29:42] Where like with the VPS, if you're having issues with your resources,
[29:47] you're shit out of luck. Like go figure it out yourself,
[29:49] you have to have more of an admin. And I believe it was the same with a dedicated server.
[29:55] - Yeah, that sounds about right. Generally with VPS, you're gonna take more ownership
[30:01] of setting it up yourself. That said, I honestly would never recommend
[30:09] using like any of the big WordPress hosts, like GoDaddy, Bluehost, SiteGround, et cetera,
[30:17] I wouldn't recommend doing a VPS through them. So actually I guess I should have covered this in the intro,
[30:25] but before I got into full stack development, for a while I built WordPress sites for small businesses.
[30:33] - I never knew that, that's so cool. I always just think Roy is a wealth of knowledge
[30:40] and when I'm stuck on stuff, I just listen to everybody playing like Apex and stuff
[30:45] and when I can hear that there's a break, I'll just ask them questions while they're doing that.
[30:49] So I'm just like, so you see you just knowing lots of stuff, but that makes a lot of sense.
[30:54] - Yep, so I still have a few clients that I'm handling their sites for.
[30:59] They'll be moving to other people in the WordPress field by end of next month 'cause I've been,
[31:08] obviously I've been away from doing WordPress stuff and I'm just kind of cycling that down.
[31:12] But for years now I've had my own VPS from DigitalOcean running, it's got like ridiculous uptime.
[31:21] And then I use a service called RunCloud, which is kind of targeted towards WordPress users
[31:30] and it manages the VPS for me. So it sets up user accounts, it sets up database stuff,
[31:38] it sets up web applications. It's like cPanel, but for VPS.
[31:49] And so it just makes it really easy to manage the server side of things.
[31:53] I can actually, I don't know if I'm sharing. Yeah, let's share the screen.
[32:01] I can share this. - And thank you, Ryan.
[32:11] I appreciate it. Find out if they're still learning cursive.
[32:17] - And that I think is another question that I'm gonna write down for a little later on
[32:25] is, let me grab that. - So this is my RunCloud dashboard.
[32:33] I still just have three client sites here. So it's just, it's winding down.
[32:39] And then what I have, you can see I'm running phpMyAdmin and I've got like a tool installed here
[32:46] to let me manage those sites. I used to have a lot more sites,
[32:50] so this would let me manage. Like I think I had 25 sites at one point,
[32:54] so let me manage them all at once. But I can go in here and like,
[32:57] I can go in and add a new database for a new site. - Oh my gosh.
[33:01] - Add a new system users, change passwords. And then I set up SSH so that I can connect to the server
[33:12] and then web applications. So this is, you know, creating the actual web applications.
[33:16] Like if I do deploy a new web app, I can go WordPress or phpMyAdmin
[33:20] and then, you know, give it a name, give it a domain, et cetera,
[33:26] and then deploy it with backups and everything like that. So it just, it manages everything.
[33:31] I can choose my php version, all this stuff in here. - Do you want to know something really funny
[33:36] that just clicked? - Sure.
[33:40] - Okay, so I knew from my time at GoDaddy that, you know, you would in like something
[33:50] like manage WordPress or cPanel or any of these, they had a database, MySQL,
[33:56] and then they would, you'd have to log in to phpMyAdmin to go manage the server or manage the database.
[34:04] Why did that not click four weeks ago when I started learning Postgres?
[34:09] You have to have the server. You have to have the client.
[34:12] - Yeah, when something like that clicks, you're like, that's so obvious in retrospect.
[34:19] - It is, it is completely obvious. And I'm just like, really, Jen, really?
[34:24] Like, oh my God, that's so very silly. - Well, I use Postgres as my database in most cases.
[34:33] Postgres clients definitely aren't quite as nice as phpMyAdmin, phpMyAdmin for MySQL
[34:43] and MariaDB databases is really, really good. - I will hopefully remember to look that up later on
[34:55] because I feel like that is definitely something to look into.
[35:01] One thing that is also coming to mind is that you were talking,
[35:08] I feel like I need to ask you first about dedicated server and then I will go back to asking you about.
[35:15] - Dedicated server really is just go-daddy, upselling services.
[35:24] I think, just looking here, I'm pretty sure that the best way to think of
[35:31] dedicated server is just, is this, yeah.
[35:38] So you may hear this term called bare metal servers and essentially what that is,
[35:44] is you're renting the hardware, the bare metal, 'cause servers are made of metal plus PCBs
[35:53] and silicone and other stuff, but metal. And then you choose what operating system,
[36:00] you build your server from the ground up. It would be like you going to the store
[36:04] and buying the parts for a computer, right? And they slap together the computer
[36:09] but they don't put any software on it. You bring it home and now, do you install Windows?
[36:13] Do you install Linux? Do you install something else?
[36:17] Which version do you install? Which Linux do you install?
[36:20] - So this one, y'all, I talk about Tyler on again, off again but that's my partner for the last 30 years, yay.
[36:31] And he also used to work at GoDaddy and was a lot more into the technical side of things
[36:39] but it was more of the, it's hard to compare it to what I'm learning now
[36:45] 'cause he went in a completely different direction and it, but I know that I can ask him
[36:50] about the dedicated server and I think this is a good way that I can knowledge check
[36:56] because I'm like, I think so, but I feel like it still wasn't like bare metal.
[37:01] It was like, they just had a more allotment. I don't know, I don't remember.
[37:07] I'll have to ask him about it but you still need to have somebody to log in
[37:12] and set up and manage all of it. It's not something that a hosting provider would do.
[37:19] - For bare metal, no. - Okay, so this is making sense.
[37:24] So I guess I didn't need to move that all the way over. We'll move that back, great.
[37:29] - Actually, looking at GoDaddy, they do offer a fully managed one where they manage it
[37:35] but yeah. - There's still stuff they didn't manage,
[37:38] at least back then when they had fully managed. - Well, I mean, reasonably,
[37:43] there's a point where you wanna do stuff that they just don't deal with, right?
[37:47] But that's kind of a different discussion. - So would you say that DigitalOcean
[37:56] is kind of almost an in-between before we go to Vercel and Netlify?
[38:02] Because DigitalOcean, can they, because they can do Docker as well, right?
[38:09] You can install Docker on DigitalOcean? - DigitalOcean, let's not call DigitalOcean an in-between
[38:16] because DigitalOcean offers a few different things. They offer VPS.
[38:22] They offer a kind of Vercel Netlify-like service. It's definitely not as mature or as involved.
[38:32] And then yeah, you can do Docker and stuff like that. So it's its own one.
[38:42] But I think before we go any further, there's still a couple of things we wanna touch on.
[38:48] So when you're talking about... Nice, soy milk, yeah.
[38:55] I mean, if you saw what I was sharing there with RunCloud, that was off DigitalOcean, all those sites were on there.
[39:00] So I definitely use DigitalOcean a bunch myself too. Yeah, I didn't configure it myself.
[39:08] I couldn't be bothered. I just let RunCloud handle it
[39:10] so that I could save time and money and sanity. But I've set up Nginx a few times.
[39:16] But yeah, so when you talk about GoDaddy, if you talk about a VPS, a lot of hosting options,
[39:23] what you're talking about is a single server in a single location somewhere in the world.
[39:28] For example, my DigitalOcean VPS is in Toronto, Toronto, Canada.
[39:36] So if someone was trying to connect to my server from California or further away, like Australia,
[39:47] or Europe, there's gonna be a delay because while the internet's fast,
[39:52] it still can take a chunk of a second to make that transit per file that's required
[39:59] for requests that's made. And that adds up, right?
[40:04] So there's all sorts of things that can affect performance.
[40:08] One of them is just waiting as the client to get a response from the server.
[40:12] And the further that that response has to travel, the bigger that delay is.
[40:17] When you start talking about performance for websites, you'll see things like time to first byte,
[40:23] which is essentially, you've heard that term before? - Yeah, and then we always had to do a, oh God.
[40:33] It was in, what was it called? Where we had to have them run on their computer
[40:42] if it was even hitting the site. Because whether or not-- - Probably like a ping
[40:46] or something like that. There's a bunch of words you could've used, yeah.
[40:49] - Yeah, something like that. Ugh, ugh.
[40:52] - Time to first byte is a good metric. What time to first byte is,
[40:56] is I send a request to a web server, what is the time in milliseconds
[41:03] until I get the first byte of a response, the first hit of a response?
[41:08] 'Cause that time to first byte, let's say you're going from Australia
[41:15] to Toronto, Canada and back, that time to first byte could easily be 500,
[41:20] yes, exactly, the first taste of a byte. That time could easily be 500 or more milliseconds.
[41:26] It's like that's a significant travel time for data, depending on the user network, depending on the server.
[41:34] Some of that is how quickly the server responds when they get the request.
[41:39] But the key there is that time to first byte is time before the user starts to get any information.
[41:47] And the longer that time is, the longer the delay will be for any request.
[41:51] Now, if you think of a WordPress site, the content, right?
[41:58] The index page, the blog articles, the WooCommerce products, the whatever, right?
[42:04] That stuff is all dynamic. And it updates sometimes frequently, sometimes infrequently.
[42:11] It depends on the site. Sometimes yearly, it depends on the particular site.
[42:16] But other things don't update. There might be a new version, but it's a separate version.
[42:25] That's images and CSS, right? CSS can get updated, but essentially we tend to treat it
[42:34] as a new version for the sake of caching. And then images, same idea.
[42:40] Something to be aware of when we talk about this is if you link to the same image, right?
[42:49] If your browser links to the same image and it already has a copy, it'll say,
[42:56] well, I've already downloaded a copy. I'm not gonna download a new copy.
[42:59] Same with JavaScript files, same with CSS files. So when we get to JavaScript tooling,
[43:07] one of the things that happens is when we generate the CSS files, the JavaScript files,
[43:13] the tooling gives it a hash code in the file name. So the file names are always different.
[43:20] And the browser will update the, or get the new version of the file anytime you change.
[43:28] If you're just editing a CSS file, the browser won't automatically update it.
[43:33] But anyway, the key is most of this stuff doesn't change often or at all.
[43:38] So we start using a content delivery network, a CDN. So what a CDN is, so I have my--
[43:49] - Before we go to a CDN, just to go back to the caching and things like that,
[43:58] which ones did you say that it normally caches? Is it any type of CSS or HTML or images?
[44:06] - CSS, JavaScript files, and images. - Okay, because, is that mostly just on WordPress sites
[44:14] or would that be on any type of site? - That's the browser behavior.
[44:19] - Okay, that's, okay, cool, cool, cool, cool, cool. And that's gonna be even if they were on something
[44:28] like Netlify or Vercel or no? - Same thing, yeah.
[44:32] It's the browser-- - Browser behavior. I just wanted to make sure.
[44:36] I'll ask you in seven different ways. - The browser does it based on file name.
[44:40] It doesn't really know whether it's a WordPress site or a React site.
[44:47] It just is like, hey, that's an image and I have already gotten a copy of an image with that name.
[44:54] I don't need to grab a new copy. I'm just gonna use the saved copy.
[45:04] - And then if anybody hosts with Lipsyn, which is a podcast host, they really do it with images.
[45:13] So even if it's a brand new episode that you're putting out, if the image itself that you're uploading
[45:18] is called the same, it will use the old image and put it out to all of your other stuff.
[45:25] Just anybody wanted to know, that was really awkward when I first realized that.
[45:32] So it caches HTML, CSS-- - Not HTML, not HTML.
[45:38] - Not HTML, okay. Actually, instead of that, I am going to do this.
[45:45] So that way I can really see that it doesn't do HTML. I think I was using my color.
[45:50] CSS, images. - In JavaScript.
[45:54] - It's weird to spell out JavaScript. Okay.
[46:02] And again, just to note that, that caching is based off file name.
[46:05] - Sweet. Okay, cool.
[46:19] - Okay. So we look at the site.
[46:22] It's comprised of HTML, CSS, images, JavaScript. The CSS, images, and JavaScript don't tend to change.
[46:30] They also tend to be larger files than the HTML, which means it takes longer for them
[46:35] to get transferred over the network. So in order to improve performance,
[46:40] I have my server in Toronto, Canada. What I can do is engage the services
[46:48] of a content delivery network, and it will cache those CSS, images, JavaScript.
[46:56] It can even cache the HTML, but we'll talk about that more later.
[47:01] And what they will do, so you have content, content being CSS, images, JavaScript.
[47:08] You have delivery, which we'll talk about in a second. And then you have network.
[47:11] Network means that you have servers all over the world. Oops.
[47:20] And let me just see if I can find a quick image. (silence)
[47:28] And CDNs can also help on security, can't they? - Sort of.
[47:44] I'm gonna send this to you in the StreamYards chat, and you can open that up on your end.
[47:56] - Okay, cool. Give me a second, y'all.
[47:58] I really should have just been doing it like this from the beginning,
[48:07] but I tried to make it bigger for everyone, but it doesn't make the most sense.
[48:12] Ta-da! - Okay, so this is actually from an image
[48:17] from Cloudflare's article on what a content delivery network is.
[48:20] What we can see is you have the origin server. That's the orange one that all the orange arrows point to.
[48:25] And then you have the CDN servers. So those are the blue rectangles.
[48:30] And then you have the users with their little fake laptops. So in the case of using a CDN,
[48:36] what it does is it takes those images, JavaScript files, CSS files,
[48:41] and it stores them on all of those CDN servers. And there's more than these.
[48:45] This shows five, just so the image isn't too spammy. But it would have...
[48:54] Cloudflare has, I imagine, probably several dozen around the world.
[49:00] So what ends up happening is you're always going to be close to a CDN server or relatively close to a CDN server.
[49:08] So when you visit that website in Toronto and get the HTML file,
[49:13] and your browser looks through it and says, "Oh, I need seven images, two CSS files,
[49:18] "and four JavaScript files," the request goes to a local CDN
[49:24] that your request gets to a lot faster. It has a very fast time to first byte,
[49:30] and it delivers those assets really quickly. A content delivery network,
[49:35] so we understand the content part, the network part. The delivery part is these are optimized
[49:41] to deliver the data to the user very quickly. The whole idea is to get that content
[49:49] to the user as quickly as possible. And CDNs are used behind the scenes all over the place.
[49:57] Discord has a CDN. So anything that is like all the images
[50:02] and stuff like that that are part of Discord, whether that's user avatars,
[50:07] whether that's Discord banners, images that are uploaded into Discord itself,
[50:16] they're all spread around on Discord CDN. Amazon uses a CDN extensively
[50:26] so that they can deliver webpages very quickly. If you think of an Amazon webpage,
[50:31] it should be slow to load 'cause they have like 50 images, and they're huge.
[50:37] But their CDN delivers that content very, very quickly. YouTube is a great example.
[50:43] YouTube is delivering videos, which are huge files, but they deliver it through their video CDN quickly.
[50:49] So this is a way to improve performance. And understanding what a CDN is will help
[50:58] with when we start talking about Vercel and Netlify because they expand upon this.
[51:09] Uh-huh. - Okay.
[51:13] Oh, yay. Hello, everyone.
[51:19] How's it going? That's exciting.
[51:24] I look down, look away, and everybody comes to show up.
[51:28] I appreciate that. And hello, hello, all you beautiful humans.
[51:34] We are hanging out, talking about, oh, it's Coding Garden, yay.
[51:41] Well, Raiden, Ron, thanks for coming over. We are talking about hosting
[51:49] because if y'all wanna see a really fun tweet that I may or may not have made earlier last week
[51:59] that was slightly embarrassing of when you feel like you're getting stuff
[52:04] and then you really don't, that is what we are working on learning about
[52:09] with, and anybody that doesn't have Twitter nor wants to, this is the tweet of.
[52:18] So when something gets deployed on Vercel or Netlify, are they actually hosting the site
[52:24] or are they not because it's grabbing the content from GitHub?
[52:28] A lot of that kind of weird knowledge comes from my time at GoDaddy.
[52:35] I was there for five years. I was in hosting sales and support,
[52:39] and it was much more taught about how do you talk about it?
[52:43] How do you sell it to people that are not normally as technical?
[52:48] We'll go with that. So it was a really hard comparison
[52:52] to what I've been learning so far since having teached Gen Tech
[52:56] of this is what it actually is. And to catch you up,
[53:02] and Roy, now we're gonna see if I can knowledge check myself.
[53:05] We are going over, we started with just a bit of GoDaddy things
[53:13] so that way we could go, okay, cool. Get my base knowledge out there
[53:17] and get an understanding check of, you know, a website at least needs HTML.
[53:23] Got it. And yes, y'all, I do know about domains and SSLs
[53:28] and, you know, DNS and all that. It's helpful when talking to a customer,
[53:34] but not always helpful when I'm just trying to get,
[53:37] level up my technical expertise. So yes, we might go through some basics.
[53:43] We talked about that there's many different servers. In a past stream with Ben Gamble,
[53:49] I've talked about, I'm learning a lot more about data
[53:54] and types of data because data is one of those things
[53:58] that a lot of people talk about yet not always go into detail about.
[54:04] And you can see a bit more about that here. And to keep going down the list,
[54:13] we started talking about shared hosting. It's like when somebody decides
[54:18] that they want to sell the seats in an airplane, but then sell more seats than they actually have room for.
[54:25] Hoping not everybody shows up. And that's what shared hosting does a lot of time.
[54:30] And then we talked a bit about managed WordPress, VPS of like virtual private server, dedicated servers.
[54:38] And right now we are going on to CDNs and caching and what CDNs do.
[54:44] Is that a good recap? - Yeah, it's a solid recap.
[54:50] - Sweet, and thank you everyone for the follows. I appreciate it.
[54:55] And as a heads up, this week particularly we are talking about,
[54:59] yes, a lot of my channel is towards beginners. I'm learning all of this live.
[55:03] This week is like really, really beginner friendly because tomorrow we're also talking about what is an API.
[55:10] And today we're talking about hosting. So a little bit more of the beginner level
[55:18] than some of our other streams where we talk about, what are some of the more technical ones
[55:25] that I've talked about? I'm trying to think.
[55:27] - TypeScript for sure. - Oh yeah, we talk about TypeScript every other week.
[55:32] I really enjoy TypeScript. That one's fun.
[55:35] And yeah, yeah. So we do a lot of random topics.
[55:40] Kubernetes, Docker. Oh yeah, okay.
[55:44] Back to CDN world. All right, so we have our content delivery network.
[55:50] Cloudflare gave us this very, very lovely description of photo of how it works around
[56:03] how close you are to the original server based on a CDN will repeat it, would you say?
[56:10] - No, they literally copy the files. It's yeah, it's the...
[56:13] So like your, all the CDN nodes will have copies of those files until there's a new copy available.
[56:22] So when you, there's options for, like when you're updating your site
[56:28] to invalidate your CDN cache, which basically says, "Okay, well, let's go and get new copies of all of that,
[56:35] "all of those files." So it tosses the old stuff and gets the new copies.
[56:39] But yeah, no, I literally, the assets that are being cached on the CDN
[56:43] are copied from the origin server and then stored on the CDN.
[56:47] - Okay. - And there's, like simplifying how they get there,
[56:52] 'cause actually typically what happens is typically the first visitor from afar
[56:59] will connect to a CDN node. The CDN node will typically see are those assets cached?
[57:04] If not, then it will go and get them from the origin server, cache them and send them to the user at the same time.
[57:09] But you know, like for how it works, that's, I don't really want to get too much into that.
[57:15] The CDN is a cache, it's not, it's like, it literally is a cache, yeah.
[57:23] - No matter what, okay. - Yeah, that's the whole--
[57:25] - It's been a hot minute since I've, because I just remember having to like talk people through,
[57:33] having to clear at the CDN. But then this is, I kind of went to another question of,
[57:39] what about, SiteLock is the, I don't even know if SiteLock is still a thing,
[57:45] let's find out, is what I'm remembering as having, like it did malware, but then it also had a CDN as well.
[57:57] And it's something that GoDaddy worked with. And I don't know if that is accurate at all.
[58:05] - It looks like-- - Solutions, ooh, well, that's,
[58:12] I wanted the dropdown, thanks, but no thanks. - Yeah, so it includes a content delivery network.
[58:18] Yeah, so it does, it does a lot of security stuff, so it'll look for malware.
[58:27] So one of the things, like just as a quick tangent, one of the things with WordPress sites is a lot of times
[58:36] they're not updated regularly. And then when they fall behind,
[58:42] their plugins will have security vulnerabilities exposed, those plugins don't get updated,
[58:49] and the site is vulnerable to an attack. If you ever go and look through the logs for WordPress site,
[58:55] you'll see dozens, hundreds of scripted attacks. So the people who have malicious intent
[59:06] will just go and try to find all of these domains that they can, and will just take all of these
[59:13] vulnerability attacks and just script them, and just run them blindly against the site.
[59:18] They don't know if your WordPress site has WooCommerce, they don't know if it has PluginX,
[59:22] they don't even know if your site has WordPress. They just run a bunch of attacks to see if any of them work.
[59:29] - Is that gonna be different than a DDoS attack? - Yes. - Okay.
[59:36] - Yeah, so these ones are attempting to use the vulnerability to gain access
[59:42] or control of your site, right? So they can change the content,
[59:46] so they can display some crypto scam or whatever it is they wanna do.
[59:53] In some way, take over the site and take over the content. Whereas DDoS is, so DoS is Denial of Service,
[60:07] DDoS is Distributed Denial of Service, meaning there's multiple computers involved in the attack.
[60:13] And the whole idea with DDoS is just that it makes your site non-responsive
[60:19] so that your services can't be used by anyone. So someone was trying to DDoS ping
[60:27] over the last couple of weeks, and if they had been successful, which they weren't,
[60:34] they were not even close to successful, but if they had been successful, ping wouldn't have worked.
[60:39] It would have been non-responsive because it would have been overloaded.
[60:43] - Interesting. Okay, well, there's lots to learn there,
[60:50] and I'm just kind of putting these as side notes. Literally, they're off to the side.
[60:55] - Yeah, they're definitely tangents. We definitely wanna spend a lot on there.
[60:59] - Yeah, so if we go back to the-- - Yep, so CDM, I think we're done with, we're good there.
[61:06] I think the last piece of the GoDaddy hosting to talk about is just super simple,
[61:11] and that's how do you get your WordPress site onto GoDaddy, right?
[61:17] You set it up locally, you have it working, or maybe you just need to move it
[61:23] from one hosting site to another. You would upload that via FTP,
[61:27] which is File Transfer Protocol, and that copies the files from your computer
[61:32] or from another computer to your server. So you can--
[61:37] - Do you wanna know something really funny? - What?
[61:40] - While working at GoDaddy, I did not realize that you built things on your computer
[61:48] and then uploaded them. Like, localhost 3000 or whatever you set your localhost up,
[61:54] no idea, did not know that was a thing. - With WordPress, it doesn't need to be,
[61:58] because a huge part of the WordPress marketplace is install WordPress, install somewhere
[62:05] between five and 30 plugins, I would say, depending on your setup,
[62:11] and they take care of all of the kind of functionality, and that includes, and then you also have themes,
[62:20] which can, like the advanced themes, can let you do all of the visual configuration
[62:28] right in WordPress, so you don't need to edit CSS files, you just go into the theme file and you can,
[62:34] or the theme admin panel, and you can configure the visual side of your site.
[62:39] So WordPress allows people to build a site completely without needing to do local development
[62:48] or to do any actual programming. A huge number of WordPress sites exist
[62:54] and no one has done any programming specific to their site. Obviously, someone built all the plugins
[63:00] and WordPress and that stuff, but no one did any specific engineering
[63:03] related to their site. They just, you know, plugins were installed,
[63:07] web and interfaces, dashboards inside WordPress were used, and everything gets configured.
[63:13] But obviously, in some cases, especially bigger sites, there's lots of custom development that's done.
[63:21] And the key here is with FTP, 'cause we'll talk about it from a different angle later,
[63:32] is there has to be some way to move the files if you're doing local development to the host.
[63:38] And FTP is one option. I'm missing a word, move site to site.
[63:47] And y'all who are new to the channel, again, welcome. As a heads up, I am wonderfully, horribly dyslexic.
[64:07] And I miss words. I also misspell like almost everything.
[64:11] So if you're like, "Jen, what are you writing?" Be forewarned, I will have probably
[64:16] just didn't even realize I did it. So feel free to let me know if something is misspelled
[64:23] or missing something as I write my notes on all this, or if something is not legible.
[64:28] And again, thank you everybody for the follows. I see the last two is Mark and Lurk Mode Activated.
[64:37] I like that name. That is a pretty dope name.
[64:41] All right, so FTP move shit. We got that.
[64:47] Isn't there a size limit for FTP? Like you can't do like over 25 megabytes or something?
[64:56] - There can be a size limit based on server configuration, but generally speaking, there's no,
[65:06] like the FTP protocol doesn't have an actual size limit. - Okay, cool.
[65:15] And you said there was something else you wanted to mention about that one?
[65:24] - No, that's all. Yeah, that's just how to get the files
[65:29] from the local computer to the server. 'Cause we will kind of talk about that process
[65:35] from a different angle when we get to, when we talk about Bristle.
[65:39] - File limit. File size limit.
[65:50] Back, back, back, back, back, back, back. Okay.
[65:55] Where do we go to now? - Now we can go to Bristle.
[66:08] - Oh my goodness. Look at all these notes.
[66:12] I'm gonna, we're gonna maybe moving this stuff over. Maybe, well, that didn't select everything.
[66:21] Goodness gracious, there we go. And we'll just move it up here with everything else.
[66:27] Maybe. Yay.
[66:34] Okay, that was fun. That was shared hosting.
[66:37] - And now we're on Vercel. - Let's get excited about some Vercel.
[66:41] - So Vercel is a tool that wraps a bunch of these things together.
[66:50] And it does it to make it easier to manage your site. It makes it easier to develop your site.
[66:55] And so that you don't have to worry about a lot of this stuff.
[67:00] - Okay. - So we'll start with, we'll kind of work backwards
[67:05] because with Vercel, you're not gonna create, there's no like, when you're signing up to Vercel,
[67:11] you don't get to create a site on Vercel. - Right.
[67:18] - You know, you have to transfer something to Vercel. And the way that that's done is GitHub
[67:25] or you can use GitLab or Bitbucket, I think is the other one, I can never remember the proper name for it.
[67:31] And so this is where we talk about the difference between FTP and, you know, Git.
[67:40] So Git is a way to take, essentially to take snapshots of your code
[67:47] as you work on it. And then also to take those snapshots
[67:51] and move them to a remote repo where they can be merged with work from other people.
[67:58] So if you and I are working on something together and we have that in the same Git repo,
[68:05] and we both upload changes to the site, those changes can be merged together.
[68:10] Git tries to be smart about it. And it says, oh, well, Jen worked on index.html
[68:18] and Roy worked on index.css, there's no conflicts there. I can just merge these.
[68:23] But let's say we both worked on index.html, it'll be like, okay, well, what lines
[68:30] and what code did Jen change? Oh, she changed lines 50 to 100.
[68:34] Roy worked on 173 to 300. Okay, there's no conflict there.
[68:39] They worked on different code, I can merge those. In some cases, you work on the same code
[68:44] and then you have to do a merge conflict where you have to choose what code to keep
[68:52] or how to merge those lines. But ultimately, you end up with those different pieces
[68:57] of work being merged into one on that remote repo. And then once that's done,
[69:03] everyone who's working on the project can download the new copy via Git pull
[69:08] and everyone has the most up-to-date code. So Git obviously has a bunch of things in place
[69:15] to transfer the files from your local computer to a remote repo, which is going back
[69:22] to the servers we were talking about, you have a Git server, GitHub is a Git server.
[69:28] You could, if you had a company that was large enough or wanted to manage it themselves,
[69:33] you could install a Git server on your own computer, your own like, you know, hardware server,
[69:40] and then have your own internal repo. - Okay, so you can have, like,
[70:03] just to, because I know I was writing at the same time, to repeat that back to you, we can,
[70:10] they use a Git server and you can have your own Git server? - If you want to, yeah.
[70:17] - Like bare metal Git server or a, or just like a larger account, I guess?
[70:30] - Well, you can install it on, however you want it, you could do it on a bare metal server
[70:37] where you would have to install the operating system first, or you could do it on a VPS.
[70:41] There's certainly a bunch of different ways to do that, but you can run your own Git server if you wanted to.
[70:51] - And do you get this question of, oh, desktop, okay.
[71:02] - No, Git desktop is a client application. As far as I know, I haven't,
[71:08] I don't use the GUI ones too often, but I'm pretty sure Git desktop is 100% client-side.
[71:15] I don't think it runs any server-side stuff. - Oh, you think you can do this.
[71:27] (typing) - This is a link to the Git docs on setting up the server.
[71:36] I don't really want to go into that too much 'cause it's not super relevant to, like,
[71:40] kind of the specifics of what we're talking about today, but essentially, you're setting up, you know,
[71:48] a server using just command line Git. And then anyone can connect to that and use that as a repo.
[71:59] A huge number of people use GitHub because obviously GitHub already has a bunch of stuff
[72:07] in place to handle that. You know, you can easily set up projects,
[72:15] you can set up organizations, you can give access to people, tons of stuff.
[72:22] And then you also don't have to worry about, you know, managing all of the costs if your repo is large
[72:31] and stuff like that. GitHub is pretty, like, it's free for the most part
[72:37] if you need to pay for it. It's pretty reasonably priced as well,
[72:41] unless you get into an enterprise or whatever. If you're an enterprise, you're making enough money,
[72:47] hopefully, for your company that the cost of the enterprise doesn't even matter.
[72:51] But the key is that at some point you end up with, you know, a remote repository.
[72:56] We'll talk about it from GitHub side of things. You end up with a remote repository that has the code
[73:02] for your web app, your project in place. And usually that most up-to-date is on something
[73:10] like your main branch. So for sell, when you're setting up for sell,
[73:16] in order to make things easier on developers, to make things easier to set up for sell initially,
[73:25] and to make things easy to use for sell and to update for sell over time,
[73:32] it connects with something like your GitHub account, or specifically your repo in your GitHub account.
[73:36] So when you set up for sell, you'll link it to a specific repo.
[73:41] It assumes by default that the most up-to-date code is in main.
[73:44] You can change that. It does a really good job of detecting
[73:49] what framework you're using. So if your repo is solid.js,
[73:53] it's gonna recognize that it's solid.js. If it's next.js, it'll 100% recognize next.js.
[73:59] Because for anyone who's listening who doesn't know, next.js is written and managed by for sell.
[74:08] So they obviously make sure next works flawlessly. It'll recognize, you know, remix or anything like that.
[74:17] And then when it recognizes that stuff, it automatically will use the default build
[74:25] and, you know, build commands for that. So it configures the projects.
[74:30] Generally, if you're using like any sort of normal framework and you haven't done any sort of weird configuration changes,
[74:36] it can detect that and set that up for you. And it takes just a few seconds.
[74:43] So what Brassell will do is it watches GitHub. Actually, I'll give you a second to,
[74:53] I wouldn't say language, it's framework. - Yeah, you're right.
[74:58] - Framework or yeah, it's called framework. Technically it can also do like,
[75:03] you can technically do like create React app, which isn't a framework,
[75:11] but it doesn't really matter framework's fine. To answer Returner's question,
[75:15] you could deploy next.js very easily to, you should be able to put it very easily
[75:22] onto Vercel or Netlify. You just have to add it to a GitHub repo
[75:27] and then connect Vercel and Netlify to that GitHub repo. And it should be deployed without any issue.
[75:33] - That's what I was just thinking, because if we go to, not Verizon,
[75:41] we don't wanna go to Verizon. I used to work there too, that's fine.
[75:45] We'll just, okay, we don't need to look at that. But like, do you have Returner,
[75:54] do you have it on a server or do you have it on just local?
[75:59] Because I don't know about get desktop if it's not set up correctly,
[76:05] because it does ask you to link it to your GitHub. Like you have to authenticate.
[76:13] Sure, we're gonna say that's all right. You have to authenticate into your GitHub, for example,
[76:20] and tell it which one to load to. So that's how I have mine set up.
[76:27] And it tells me which GitHub project that I need it to go to, which repo to go to.
[76:34] - Yeah. Returner, I would say that if you're getting errors,
[76:40] there's probably a couple of things that you can look at. Number one, if you have put anything into a .env file,
[76:49] you wanna go into Vercel or Netlify to the project where you're trying to deploy,
[76:56] and there'll be settings. Jen can show us.
[76:59] She goes to, click on Website on your Vercel. - There, oh, I don't know where that is.
[77:08] There's a lot of things. - Click on Settings.
[77:10] - Settings. - And then Environment Variables.
[77:16] So if you have anything in a .env file, you would go in here in Vercel,
[77:20] and there's an equivalent in Netlify, and you would add those key value pairs in here.
[77:25] Your .env file won't be getting uploaded to, or shouldn't be getting uploaded to GitHub.
[77:33] And even if it is, Vercel won't read the contents of it. So you wanna put those .env values in here.
[77:38] That's one thing to look at. Locally, you can run your next build command,
[77:43] so that should be npm run build, or npx next build, and it'll build.
[77:50] That's the same process that happens when it tries to deploy on Next.
[77:54] The build process is different than the npm run dev, the development server.
[77:58] The npm build, npm run build is more strict and will often error out on things that the build,
[78:06] the development server doesn't error it on. So if you get errors doing the npm run build,
[78:12] you can check those errors and look at resolving them. They could be TypeScript errors,
[78:16] or things like React strict related errors, stuff like that.
[78:19] So you can take a look at that. If you can do an npm run build without errors,
[78:27] and you've uploaded your .env files, you should be able to deploy without problems.
[78:33] But yeah, I don't, certainly wanna help you,
[78:36] but at the same time, we don't wanna turn this into a troubleshooting stream,
[78:42] at least not yet, maybe later on after we've-- - Maybe later on, yeah, eventually.
[78:46] This is something that I will say that I've run into, I built my site with Astro,
[78:52] and I have had it where it would run locally, but it wouldn't deploy on Brazil,
[78:57] that's why I was just looking up my logs. And I don't remember what it was,
[79:01] but it took me like an hour to, of lots and lots of Googles,
[79:05] to try to figure out what it was, and it was like a file wasn't uploading properly,
[79:10] or something like that. I don't remember.
[79:12] But yes, it can happen, but those logs will definitely, definitely help you out.
[79:17] - Yeah, so the key with all of this is, when you're getting set up,
[79:30] if you're looking at trying to diagnose problems, one of the first things you should always do
[79:36] with any of the frameworks is run their build command. So when you run npm run dev on your Next,
[79:43] or your Astro, or whatever, locally, it runs a development server.
[79:51] A development server doesn't build the JS bundles and the CSS bundles the same way
[80:00] as you need for an actual development, a actual production server.
[80:07] - You just reminded me, sorry to interrupt, but it was, I think it was a JavaScript error
[80:15] that I had to update my JavaScript because I wasn't reading the most recent version
[80:20] of TypeScript or something like that. - Yep, it could be anything like that.
[80:25] The key is that the build step is, when you do npm run build,
[80:30] it's going to build all of those JavaScript bundles, CSS files, et cetera, the way it would for deploying it.
[80:38] So basically the difference is, when you are developing, it doesn't build those files
[80:48] because what it wants to be able to do is, on most of the frameworks, is do a hot module reload.
[80:56] Meaning when you make a change on one of your files and you save it, your development server says,
[81:03] "Oh, you changed this file," or, "You changed that file." It reads those changes and it automatically injects them
[81:10] into your development server and what you're looking at locally.
[81:16] So if you change your CSS and you save, it will automatically update your project
[81:22] and where you're looking at it locally in the browser, like localhost 3000 or whatever,
[81:26] you'll immediately see that update and be able to see what's going on.
[81:30] But part of that is because it doesn't go and build a CSS file in the sense of the way it will
[81:38] when it gets deployed. But the build command will do that.
[81:43] So it'll take and build an actual CSS file. So if you're working with, say, Tailwind
[81:50] and you do an npm run build command and you look at the build folder after,
[81:55] you'll find an actual index.css or styles.css, whatever you call it.
[82:00] You'll find that actual file with all of your styles in it. And you'll be able to take a look at them
[82:06] and you'll find the actual rendered HTML file. You'll find, like, it's gonna be a small file,
[82:13] but it'll be there. You'll find your JavaScript files
[82:17] and they'll all be in their build one. So yeah, anytime you're having a problem deploying,
[82:23] do your build command locally and check your errors because that's one of the things that's gonna happen
[82:29] when you deploy in Vercel, which is what we're gonna talk about.
[82:32] So you've set up your Vercel account and you've linked it to your GitHub repo, right?
[82:39] - Yes. - What Vercel is gonna do is say,
[82:48] "Okay, I am going to take a copy of the code "that is in the main branch."
[82:55] And I am going, pull it over to Vercel. I am going to do the npm install, install the packages.
[83:05] Then I'm going to do an npm run build or equivalent commands.
[83:14] Like, I'll keep saying npm run build, but that can be different
[83:16] depending on the framework, actually. It'll do the npm run build command
[83:21] and build the deployable assets. And then we'll take that and we will add it
[83:26] to our edge network, which we'll talk about in more detail. And we'll make that live so people can access the site.
[83:37] So if you're in Vercel, you can look at your build logs and that's the process of what it's doing there.
[83:45] - Can I just say, I feel like I wasn't that far off because it basically, I was like,
[83:50] "Yo, it's just running npm run build." - Right.
[83:54] - I just didn't know the edge network. - You also, in your original tweet,
[83:58] had thought it was running it on GitHub, which it's not. - Because it's pulling the information from GitHub
[84:04] because I didn't know about edge network 'cause I was like...
[84:07] - Well, the run build is before the edge network. - Yeah, and that's why I'm like, "I didn't know it existed."
[84:15] So I was like, "Where else could the content have come from?" - Right.
[84:19] - So that's why I'm excited. Don't mind me, yeah.
[84:21] Okay. - So, yeah.
[84:23] So then it takes those built files. So you have your core HTML file,
[84:30] in the case of something like React. Has all your CSS files, your JavaScript files,
[84:35] your images, et cetera. And it makes them available for people to visit the site.
[84:41] And so now people can visit your website and access it. Now, this is where it starts to get
[84:48] a little more complicated. Because when we were talking GoDaddy and WordPress,
[84:51] we talked about server-side rendering. Everything that's PHP is server-side rendered
[84:56] because the browser can't render it. JavaScript gets into this weird...
[85:03] Not weird, but this more complicated situation where you can have server-side rendered,
[85:08] basically like PHP. You can have static site generation,
[85:13] which you can also do with PHP and WordPress. But it also includes client-side,
[85:19] or what's often referred to as single-page applications. - Okay.
[85:26] - If you're using Next by default, it is a single-page application, a SPA.
[85:36] If you're using Astro by default, it's a static site generator by default.
[85:41] I think actually only the static site generator. So the key here is depending on the framework
[85:49] and depending on how you have it configured, the behavior can be a little bit different.
[85:53] So we'll talk about Next and it's like default version first.
[85:56] And so it's a SPA, single-page application. So what that means is there's an index.html file.
[86:03] It has some SEO stuff. And then it just has like an empty div with an ID.
[86:09] And the JavaScript that's part of React will look for that ID.
[86:13] And then the JavaScript will create all of these divs and headers and stuff like that.
[86:20] - You said it was just a single-page application? - Yep.
[86:25] Yep, that's what, like if you go and look at Next, you'll find that there's a public folder in,
[86:32] actually Next's not like that. I don't think, I can't even remember anymore.
[86:39] I've been messing around with other frameworks. I think Next just auto-generates it now.
[86:43] But you end up with just a single app, like an index page with an empty div
[86:53] where the content will be injected. And so the application will,
[87:02] which is the JavaScript, will generate the page on the client.
[87:05] So the browser is running the JavaScript. And that JavaScript says, hey, create a div.
[87:10] Okay, inside of that div, create another div and give it these CSS classes.
[87:16] And inside of that div, give it a h1 tag and then this text, like teach gen tech.
[87:23] And then close that and close that div. And then let's create another div and call that,
[87:28] give that some other CSS classes. And then inside of there,
[87:32] let's add this content for a blog post. And it's gonna render all of this.
[87:37] And then it takes all of that rendered HTML and it shoves it into that empty div.
[87:41] - Okay. - And then if the client clicks on another link
[87:49] in the application, so they wanna go to a different page,
[87:52] it renders that new page, takes all the content for that new page,
[87:57] erases what's in the div, that top level div in the index file
[88:02] and shoves in the new HTML. - Oh, okay.
[88:05] Hold on. Before you keep going.
[88:08] Let me rewrite this so I can. Okay.
[88:18] So it would be an index.js with-- - Index.html.
[88:24] - Oh, it would be index. Okay, yeah, yeah, yeah.
[88:28] Index.html. And then it would be with empty div.
[88:37] - Yep. - And then if I,
[88:41] then the rest of them would be like a .js, like it could be gen.js.
[88:47] And then it would-- - Nope, it wouldn't be anything like that.
[88:49] Nope, so that's where you wanna, this is what's complicated with SPAs.
[88:55] There would be no JavaScript files or HTML files that relate to what we think of as pages.
[89:02] It's a single page, index.html. What happens is inside of the JavaScript code,
[89:10] it says what route is the user trying to access? So slash is your main route,
[89:19] like what you would get if you went to tshendtech.com. And then there would be another route,
[89:25] slash blog or slash about or slash content. And so you have some sort of router package
[89:35] that manages that. In the case of Next, that's file-based routing.
[89:40] So people get confused with Next because you create these files,
[89:43] like, oh, if I wanna have a contact page, I create a file called contact.js or jsx or ts or tsx,
[89:53] but there's not actually a page. When that next application is built,
[89:58] if it's being built as a SPA, all of that JavaScript just gets moved into a bundle.
[90:06] And then there's router that says, oh, you're trying to go to slash blog.
[90:10] We'll render the HTML for slash blog, but there's no corresponding file.
[90:15] It's all handled in JavaScript. - So where would you write it?
[90:20] - Write what? - The information that it's rendering.
[90:25] - You write it in, in the case of Next, you would write it in a blog.ts file
[90:32] or a slash blog slash whatever file. But the key is that during the build process,
[90:40] all of that JavaScript gets amalgamated into just bundles that get loaded by index.html.
[90:50] - Okay, so I think I understand this better now. So if it's gonna be a blog like this,
[91:01] it would be, we'll say, teach in tech.js.
[91:10] And then whatever is here, let me change colors.
[91:16] Yay, colors. Let's do purple.
[91:20] Whatever is written in file. Goodness gracious, please ignore the dog.
[91:33] And yay, thank you for another follow. Whatever is written in the file
[91:38] will be built in the index.html in that dev. - Not quite.
[91:48] So let's move that blog thing down. - Okay, give me a second to get the dog out of the room.
[91:54] So just a sec. Doggo, you need to go this way.
[91:57] Oh, good girl. She is an old lady, so she's gonna be old lady.
[92:06] There, kicked her out of my office for now. Okay, so you said move the blog?
[92:12] - Yeah, move that down so we have some room. - No, I gotta move my P back.
[92:18] There we go. - All right, so what happens is
[92:21] when we do the build command, you'll end up with something like index.js.
[92:26] So we'll call it index.js, it may, it can be named differently,
[92:29] but index.html will load index.js. - Okay.
[92:35] - So you can do like, I would do like a little like L arrow down from index.html and say, index.js.
[92:42] And then you can just, in brackets, say like create a jerk build step.
[92:47] (indistinct chatter) - Okay.
[93:04] - And then everything below, so your blog page, your index,
[93:08] your main page, your video page, your blog articles, your contact page,
[93:14] everything else during the build step will get turned into JavaScript
[93:19] and get put into index.js. Again, simplifying that process
[93:24] because it will probably split index.js into multiple files to keep them from being too big
[93:29] and there'll be tree shaking and stuff like that. But we don't need to get into that in this case.
[93:35] We just, the general sense is all of that React code is converted to JavaScript, plain JavaScript,
[93:45] and put into index.js. - Okay, this is totally making sense.
[93:51] I'm just gonna move stuff, so. Okay, and then you said,
[93:57] let me move these notes to another page. No, down here.
[94:04] Cool, thank you. And then you said,
[94:09] anything else you wanted to talk about after the SPA? - Yeah, so you now have the index.html file.
[94:20] You have your JavaScript files. You have your CSS files.
[94:25] So those get served to the client. So the client gets the index.html file.
[94:33] It says, hey, go get these JavaScript files. Go get these CSS files and those images files.
[94:38] And all of that code is constantly executed on the client, right?
[94:42] So SPAs are client-side. So everything is on that user's computer.
[94:52] This is one of the reasons that, for example, something like Prisma won't run
[94:58] in this part of your application, because it's client-side.
[95:05] And in order for Prisma to run, you would have to send every user
[95:10] the username, password, and access information to your database.
[95:13] And then someone who's being malicious could just read that and be like,
[95:17] oh, well, there's the username and password to access Jen's database.
[95:21] And I can just go in there and delete her stuff or modify it.
[95:26] And now all of a sudden, her front page shows pictures of Elon
[95:28] and cryptocurrency scams. And Jen's like, oh no,
[95:32] that's not what I wanted to show the world. That sucks.
[95:36] So, yeah, this is all on the client-side. - And again, client-side means their--
[95:43] - Your browser, specifically browser. - Okay, cool.
[96:02] So now, JavaScript applications can also be server-side rendered.
[96:10] So server-side rendered means that when a request comes in for a particular page,
[96:19] the server will load the JavaScript for that page and render it on the server.
[96:29] So this is similar to WordPress, right? When you visit a page for WordPress,
[96:35] the web server renders that page and sends it to the user.
[96:39] So the same process is happening here. You know, obviously different language and whatnot,
[96:44] but the same general process. It is taking that,
[96:51] that route that you're asking for, so /blog/tjt and says,
[97:03] "Hey, what JavaScript do I need to render this page?" Okay, let's execute that JavaScript,
[97:12] create the index.html, or not the index, the blog/tjt file,
[97:19] and then send that to that complete HTML file to the user. Okay, so, and hello, hello, happy to see you.
[97:33] Okay, so I think where I'm a little stuck, and I honestly don't know if I've had this on the show,
[97:42] which is something that, of course, we hear about client-side or server-side,
[97:47] or in my head, hydration goes into this. - We're about to talk about hydration.
[97:53] So server-side rendering will have hydration. We're gonna get there in a second.
[97:57] I wanted to make, just waiting for you to kind of ask the questions about server-side rendering.
[98:02] - I guess what I don't get is when it's on the client-side, does that mean local only?
[98:09] - What do you mean by local only? - 'Cause you said it has to do with their browser.
[98:14] I guess where I'm having a hard time picturing is if it's on client-side,
[98:23] like, it's not gonna load 'til it gets to their computer, and then it's gonna load where this server-side
[98:32] is gonna load before it even goes through the interwebs. After interwebs, before interwebs.
[98:42] - Before, yep. - Okay, that is a very simplified version of it.
[98:47] - It's super simplified, but so here's why this matters, and why server-side rendering
[98:52] is often chosen for performance. So let's say that this SPA app
[98:59] needs to get information from a database, right? It needs to load blog posts,
[99:05] it needs to load user information, et cetera, right? Or whatever the case is, right?
[99:10] It needs to load information from a database. As we said, generally it won't access the database directly
[99:16] because of security issues. There are a few exceptions, like you can do Firestore,
[99:22] but generally you don't access your database directly from the client-side.
[99:28] So in this case, right, with the SPA, wait, why do you have, oh, right, sorry,
[99:38] I see how you're writing it, it's confusing for a second. So in the case of the SPA,
[99:43] you go and visit, or I go and visit TeachGenTech, right? - Mm-hmm.
[99:49] - It sends me the HTML, it sends me those JavaScript bundles, CSS bundles, initial images.
[99:54] My browser starts to render that JavaScript, and it says, oh, well,
[100:00] in order to display this page correctly, you need to go and get the 10 most recent blog posts.
[100:05] So now my browser says, okay, based on the JavaScript, I need to access the web server,
[100:12] the API that you're gonna talk about tomorrow, so we don't wanna go into this too much,
[100:15] 'cause you can ask all those API questions tomorrow. It'll access the API, which will be your server side, right?
[100:23] So this is where we talk about full-stack development, right, so full-stack development,
[100:29] front-end development, which is building the pages, you have back-end development,
[100:33] which is the server that interacts with the database or third-party APIs,
[100:38] and then you have full-stack that does both, so-- - As a side note, just 'cause Ilyan,
[100:46] Ilyan, dammit, I will get it right one of these days. This is his theme.
[100:55] - Oh, okay, yeah, that's right. He was the one who made that theme nice.
[100:58] - Yeah, yeah, eventually he will be on the show. We will figure out schedules,
[101:01] but I just wanted to showcase that because it's very exciting.
[101:05] I really like this theme. Okay, please continue.
[101:08] - Right, so this SBA says, okay, well, I need to contact the API, the back-end server,
[101:14] and get the 10 most recent blog posts. Oh, I also need to go and get,
[101:18] you know, whatever, some of, you know, her three most recent projects.
[101:27] I need to get her last five tweets, whatever the case is, right?
[101:32] So it has to go and get this information. So now it has to send requests to your back-end server
[101:39] for that information. Your back-end server gets that request,
[101:43] processes the request, and sends that information back, usually in the form of, like, JSON.
[101:51] And then that client will read that JSON, take that information, so those 10 blog posts,
[101:58] and it will say, okay, here's the information you asked for,
[102:04] and it'll render, you know, your blog preview 10 times, one for each of the posts.
[102:10] So now if you're thinking about this, in terms of, like, how does this affect performance,
[102:18] the user had to request the JavaScript first. It had to be sent to the user.
[102:24] Before the page could be rendered, another request had to be sent to the server
[102:29] to go and get this blog post information to get these projects, right?
[102:34] And then, so the client has to sit and wait, right? So the client's waiting while that process happens,
[102:41] and that information returns. - Okay.
[102:45] - Then it can render that information, and hopefully render the whole page.
[102:48] Hopefully there's nothing else it needs to do. So server-side rendering, what happens is,
[102:55] because you're rendering on the server, the server immediately says, I need 10 blog posts.
[103:02] Now, in most cases, it's gonna be faster for the server, in this case, like Vercel,
[103:10] to contact the database, which is gonna be on another server, right?
[103:15] So you're learning MySQL, you might look at a database that's hosted on something like PlanetScale.
[103:23] - Yeah. - Right? So your database is on a different physical server
[103:26] than Vercel, it's on this PlanetScale server. It's almost for sure faster for Vercel
[103:32] to contact your database than the client. Vercel's already on enterprise-level networking,
[103:39] PlanetScale's on enterprise-level networking, the user's on whatever networking they have,
[103:45] some DSL package, or their phone, or whatever, right? So, oh yeah, of course,
[103:53] should actually not say PlanetScale, 'cause you're-- - It's okay, I wasn't gonna correct it.
[104:00] - But no, you work for a company that provides that, so yes. - What's the, it's Evian?
[104:09] - Ivan, like I-V-A-N, just-- - Yeah, I would never guess Ivan looking at that
[104:15] for being a guy from Toronto, Canada. But anyway, Ivan, yes, so yes.
[104:23] - It was a made-up word, it's not something that means something in Finnish or anything.
[104:28] - Oh, okay. - And so yes. - It probably makes more sense to pronounce it that way
[104:32] to Finnish people than me, I would guess, but maybe not, who knows?
[104:37] - I don't correct people when they say it, I'm just like, yeah, whatever, because--
[104:42] - Yeah, if you didn't tell me that was Ivan, I would, Ivan would be like my 50th guest probably,
[104:47] but anyway. - Yeah, no, everyone is like that, that's why I don't even, like,
[104:52] okay, so-- - So Vercel's gonna be faster to contact Ivan's DB, get that data,
[104:58] and it's almost for sure gonna be faster to render the page than the client's browser, right?
[105:04] That's not always true, sometimes the user has a monster computer at home, and they know what they're,
[105:08] you know, they've got everything optimized and stuff like that, like my computer is ridiculous
[105:13] 'cause I have it optimized for gaming, and it's, I spent way too much money on it,
[105:16] but that's not the average person, and certainly, like, your phone isn't gonna render faster
[105:20] than, you know, a server. So Vercel says, oh, I need these 10 blog posts,
[105:28] hit up Ivan, get the 10 blog posts, render the page, and then send that rendered HTML file
[105:33] to the user, so what you haven't had is that extra back and forth, right?
[105:37] The user didn't contact Vercel, get some information, and then have to contact Vercel again,
[105:43] who then contacted Ivan, who then got the database information, who then sent it back, right?
[105:48] So there's a whole lot more back and forth within SPA, potentially, whereas with server-side rendering,
[105:54] a lot of that initial back and forth is handled between servers before the page is rendered.
[105:59] So that can be a lot more performant. - I'm giving up on my squares, but--
[106:14] - What we want to do is that one that comes down to render page,
[106:17] you wanna go back to, you wanna have that arrow go back to Vercel, and then an arrow from Vercel
[106:22] to say render page, but yeah. It's good.
[106:26] - What, okay, that's where, sorry, I didn't know where my, okay, there we go.
[106:30] So it goes like this, and then like this, and then it will send a different arrow,
[106:42] we're gonna do pink, like this, back to Vercel, and we're gonna erase this,
[106:50] and then we will do a orange one that is here to here. - Yep, that's--
[106:59] - Yay, and a very ugly way of doing it. I will rewrite it later.
[107:04] - No, that's all good. The key here is you only have that one orange arrow
[107:07] from Vercel to the user. - Oh, where, okay, so--
[107:12] - Where in the SPA, you would have Vercel to the user, user back to Vercel, Vercel to Ivan,
[107:20] Ivan to Vercel, Vercel back to the user. - I feel like it's starting to click,
[107:26] but now I really wanna draw these out because these little images, for some reason,
[107:33] really help my head understand stuff. - Yep, while you draw that row,
[107:37] I'm just gonna step away for about 45 seconds. I'll be right back.
[107:39] - Do it, and then we're gonna see if I got it right. We'll find out.
[107:44] - Yep. - Well, let's see.
[107:50] I feel like we can definitely draw some bigger squares. So, so we have the browser.
[107:59] Let's say browser and then it has to go to Vercel. And then it has to go to Vercel,
[108:13] which is the server, and then it has to ask for, I'm gonna say this is the order.
[108:31] We'll find out. Blog post, 'cause I wanna see what that blog post is.
[108:39] It's a new blog post. And then we have to do Ivan Postgres database,
[108:59] and then it needs to go back to Vercel, I think. - Should be Vercel to Ivan.
[109:09] Ivan to blog post, blog post to Vercel. - But where does it put the request?
[109:17] - Well, so what's gonna happen is you're gonna have the browser go to Vercel.
[109:26] Vercel back to the browser. So I guess the blog post square,
[109:33] is that the request for the blog post or the content for the blog post?
[109:36] - No, it's the request. - Okay, so it should be arrow from browser to Vercel,
[109:42] then arrow from Vercel to browser. - And to Ivan.
[109:46] - No, then arrow to the blog post request, or Vercel. I guess it depends how you wanna map it out.
[109:57] I would go blog post request, then to Vercel, then to Ivan. - Oh, okay, okay, hold on.
[110:04] That makes sense. What is one of you doing here?
[110:11] Welcome to your new home. And then you go to Vercel.
[110:14] We're just gonna make a lot of boxes. And then--
[110:18] - I would keep Vercel where it was. That's a good spot for it.
[110:23] - Okay, so we got Vercel. So to double check that, I know it goes from,
[110:33] we request the blog post. - No, no, so the initial one is browser to Vercel.
[110:42] And then Vercel back to the browser. - Okay.
[110:47] And then, oh, because it has to check it. - Yep.
[110:55] - And then we do-- - So now when it's executing the JavaScript,
[110:58] it says, "Oh, crap, I need 10 blog posts." So now you have that blog post request.
[111:04] And then that goes to Vercel. - Into Vercel.
[111:11] - And then Vercel says, "Okay, I need that information from Ivan."
[111:21] - And then we go to Ivan, back to Vercel. - Back to Vercel, and then Ivan says,
[111:27] "Here's the information." And then Vercel sends it back to the browser.
[111:32] I guess you could send it through the blog post request if you wanted to, but yeah.
[111:37] - That's not complicated at all. - Not at all.
[111:47] And remember that that process occurs for every piece of data you need from your database,
[111:52] which on a more complicated site could be many pieces. Yeah, we're about to do SSG.
[111:58] We'll just verify SSR first, and then we'll get to SSG. - Okay, let me put that this is a spa.
[112:18] And this is... And this would just be called SSR, right?
[112:29] - Yep. - SSR.
[112:32] Give myself a nice thing. Okay, there we go.
[112:37] I'm slowly, slowly picking up what you're putting down. - Yep.
[112:41] So we can see that SSR is, has the potential to be a lot faster.
[112:46] One, because there's less back and forth. And the back and forth that occurs
[112:51] is at the very start of the process and between servers. So you end up being able to render the page a lot quicker,
[112:59] and certainly with less network requests, especially between the user and Vercel.
[113:04] So the last part of Vercel before we move to SSG is hydration.
[113:11] So, hydration is essentially, like you, so the first part of SSR
[113:18] sends an HTML page to the user, right? There's no JavaScript yet.
[113:24] - Right. - So, hydration is essentially then taking
[113:30] and saying, okay, we've served a static HTML page, but we need to add that Astro, or that React,
[113:39] or that solid JS code. So it comes in a step later.
[113:46] So the HTML page gets rendered on the user's browser and they're like, oh, cool, here's the content.
[113:53] They start to scroll through it. And then what's happening,
[113:57] and the next step in the background is the server and the browser are grabbing that JavaScript
[114:03] and it basically attaching it to the HTML. So that all of the interactivity that you would want
[114:11] from React or whatever the case is, is now present. So you might have interactivity on like a button.
[114:18] It gets attached as that React code comes in. - Okay.
[114:25] Give me a second 'cause I'm also just trying to understand where we're at right now.
[114:40] 'Cause, okay, so we have, before the user browser, all of this happens.
[114:48] So it goes for, so, yes, I'm rewriting the other one that we already have to 10 blog posts,
[114:56] or I'm just gonna say blog post request. Let's see if I can actually, right.
[115:08] And then it goes to Ivan, the database, and then back to Vercel,
[115:22] and then it would render the page and be in the browser.
[115:28] Okay. So let me draw my arrows, browser.
[115:35] Goodness gracious, so we're gonna have some hot pink. It's gonna be great.
[115:43] We go to a dish, and then we go like this. And then we're gonna have a different color
[115:48] that will go all the way back to Vercel. And we will do green.
[115:59] Sure, why not? Then you render, and then you go to the browser.
[116:05] Thank you for holding. That was a lot.
[116:08] And now when we're talking about hydration, hydration will add it to like after the database part,
[116:18] or would it be like-- - After the browser.
[116:25] - After the browser. - Yep, so the user, in this case,
[116:28] the user's now received an HTML file, and it has all the blog posts and all the content, right?
[116:35] It's a complete page. - So I'm just gonna say browser HTML then.
[116:43] And then after that is, then all of this will be added with like,
[116:55] you said JavaScript and CSS? - No, it's all the JavaScript.
[117:00] CSS has already been sent, images, all that in the HTML. - So I'm just, I know this is extra,
[117:09] but HTML, CSS, images, already sent. So the JavaScript is now going to,
[117:28] it's gonna go out to the JavaScript and then go back to the browser?
[117:32] - Sort of, yeah, yeah. It's kind of happening in the background.
[117:37] So, and that's the important thing to understand, is like when you're looking at a server-side rendered page,
[117:44] you're getting, the user's getting an HTML page and it pops up quickly and they're like, oh, cool.
[117:51] And then, you know, in the background, as a follow-up step, hydration occurs.
[117:57] And that's for Vercel or the host, finishing the request and sending the JavaScript
[118:05] and the JavaScript attaching itself to the HTML page. Because essentially React,
[118:13] like in a production environment has a bunch of event listeners attached to the page.
[118:23] And those event listeners point to different parts of, different pieces of JavaScript.
[118:27] So at this point, it's rendering that, like executing that JavaScript
[118:33] and attaching those event listeners and making the page interactive in the way
[118:38] that you would expect for React or whatever it is. - Okay, we said that the SPA is probably like a Next.js,
[118:46] so server-side would be like React? - Nope, Next.js does all three.
[118:52] That's one of the reasons I'm using this example. The default behavior for Next.js is SPA.
[118:58] You have to choose to do SSR or SPA in React, in Next. And like React, like if you use React with no framework,
[119:10] no Next, no Remix, no Astro, et cetera, you use just like vanilla React, it is an SPA.
[119:18] - What about, what's Vite? - Vite is an SPA.
[119:26] You can, there is some server-side rendering. I don't know if there's any SGA or SSG with Vite offhand.
[119:35] - I ask because I, one of the first ones that I did with Anthony Campolo was Vite's a build system
[119:44] because we did a React app with Vite and Vercel. - Yep, yep.
[119:53] - Generally speaking, most people will treat Vite as a build system, which is build your React app
[119:59] and then you, it will build the JavaScript bundles, the CSS bundles, et cetera.
[120:08] It's very fast and very efficient at doing it. - Okay, okay.
[120:15] We're gonna ask about build systems later. Let me go put that on my...
[120:19] (mumbles) That's not how you say like.
[120:28] It helps if I can... Eats.
[120:32] Okay, so, cool. I feel like I'm getting it.
[120:40] All right, and then we have SSG after this? - Yep.
[120:47] - Okay. - I honestly had no idea any of these really existed.
[120:53] Like that they officially existed. I've heard of them, but didn't know what they meant.
[120:59] I'm so excited. So much drawing today.
[121:03] All right, so let's get some SSG. Server-side gathering?
[121:09] - Generated. That's not server-side, it's static site generation.
[121:14] - Oh, okay. (mumbles)
[121:18] - So is stuff like Website Builder or Wix and that kind of stuff, is that SSG?
[121:30] - Sorry, Wix or what? - Like GoDaddy's Website Builder,
[121:35] Wix, Squarespace, that kind of stuff? - No, I don't think any.
[121:41] I don't know actually, specifically how they work under the hood.
[121:44] I don't really look at any of them. I think the answer is probably no for all of them.
[121:48] They're probably more server-side rendered. - And Rex just said no as well.
[121:54] So thank you, Rex. Okay, so you're saying that they are probably SSRs?
[122:00] - Yep. That's my guess.
[122:02] Like I don't, especially with GoDaddy, I really know nothing about GoDaddy's Site Builder
[122:07] and Wix and Squarespace. I'm pretty sure that by default they're SSR,
[122:12] but they might have some form of SSG. I'm not sure offhand.
[122:18] - That's why we will put Probs SSR. We're not gonna--
[122:23] - Also probably doesn't matter 'cause you probably have no choice with them.
[122:25] So like if you use them-- - It's more for me to understand.
[122:28] - Right, yeah, yeah, yeah. - Yeah, not to try to fix stuff, just understand.
[122:33] Okay, so static site like Astro? - Astro is, yep.
[122:40] Astro is an example. And then Next allows you to do static site generation.
[122:44] So static site generation is this idea that your site has information that you're loading
[122:50] from a database or third-party APIs, but that that information doesn't change very often.
[122:56] So your great example is like your or my personal sites. We don't update our projects or our blog posts
[123:06] all that often. I certainly don't.
[123:08] - I should be. - Well, you probably should be, but we, most people don't.
[123:13] So, and I mean, even in the general sense, even if you write a blog post a week,
[123:18] that's still really infrequent for this stuff. So your site isn't changing.
[123:25] Certainly every hour, every day you don't need, you don't need to go and have your users
[123:33] querying your database to get updated information 'cause you aren't writing blog posts every hour.
[123:40] Contrast this to a similar idea, like a new site, which is essentially like very similar to a blog site
[123:49] in kind of a general sense. It's a whole bunch of stories, posts,
[123:56] but a new site is gonna be adding new sites every few minutes, potentially,
[124:02] or more frequently, depending how big the site is. And they're gonna be editing past stories.
[124:06] So their content is gonna be a lot more dynamic than your personal site.
[124:11] So blog, your personal site, portfolios, blog sites are good examples of sites
[124:17] that can be relatively static. Docs sites, the docs for Astro, for Next, et cetera,
[124:24] tend to be relatively static as well. Stuff like that.
[124:28] So the idea with static site generation is when you do your build step,
[124:36] all of the pages that you want to statically generate are created then.
[124:41] So the interesting thing with Next is you can choose on a page-by-page basis
[124:50] which are SPA, which are SSR, which are SSG. So you could have three different pages
[124:56] in your next project, and you could choose a different behavior for each one if you want to.
[125:04] So in the case of my portfolio site, most of my portfolio site is statically generated.
[125:12] All my blog posts, my projects, the index page, et cetera. The one page that it isn't is,
[125:18] I have a page that shows Spotify information, what I've been listening to, what I'm currently listening to
[125:24] if I'm listening to something, you know, popular albums. That page handles an SPA
[125:31] because it wants to get updated information. So when you're setting up Next
[125:39] and you have a bunch of pages that you want to be statically generated,
[125:45] you set them up to be statically generated. And when that build step occurs,
[125:49] that's when they're created. So this happens well before the user would request the page.
[125:55] - Side note, that does not go to this page, but it's going to help,
[126:01] especially with the conference I have going on. Is Next a meta-framework?
[126:10] - Yeah, I think- - Because Next is to react as Next is to view.
[126:19] - Honestly, the whole framework, meta-framework, meta-meta-framework stuff people chat about,
[126:27] it's like, I don't know. Next is definitely a framework.
[126:32] I don't know if it... Yeah, I think it does
[126:37] 'cause I think it goes beyond just React. I think meta-frameworks are stuff
[126:41] that include routing and whatnot. But yeah, Next does a ton of stuff
[126:53] and it's getting even more complicated too in the future. - That's okay.
[126:59] I wrote my note to go look into it later. Okay, so I like that I can,
[127:04] I wrote down that it can be mattering on the page, it can be all of those.
[127:09] Ooh, excuse you. I don't want this.
[127:12] Done, goodbye. So something that I just realized
[127:19] that I don't think I understand from these graphics is what is considered the build step?
[127:27] That's that npm run build. So we talked about how Vercel, when you're deploying,
[127:33] will grab a copy of your repo, typically the main branch.
[127:38] - Right. - It'll do the npm install.
[127:40] It's right there at the top of your page, by the way, if you didn't see it.
[127:43] - Yeah, yeah, yeah. I guess, where do I go from as a...
[127:49] Oh, I forget I can do this. Where does this go in this?
[127:55] - After. - After Edge Network.
[128:00] - This is after Edge Network, okay. - Yep, same with SSR.
[128:03] - And SSG? - SSG is actually split into two parts.
[128:09] So there is, during the build step, there is create the static pages.
[128:17] So create HTML versions of the pages. And then those get put on the Edge Network.
[128:25] So the comparison is, if you do next as an SPA, you'll end up with one HTML file, that index.html file,
[128:34] your JavaScript files, your CSS files, and those will go on to the Edge Network
[128:41] and get served to the users. In the case of SSG, you could have dozens of HTML files
[128:52] for all the pages that you marked to be statically generated. And then you may still have some other,
[129:02] like you still may have your... You'll obviously still have your index.html file.
[129:06] You may have some pages that are handled outside of SSG, like I said, 'cause you can do a page by page.
[129:13] So those will be handled by that index.html file and your JavaScript.
[129:19] Whereas the ones that were statically generated, like blog.html or contact.html,
[129:27] those will be served as HTML to the user from the Edge Network.
[129:32] - And then that's as far as I got on what you just said. - Yeah, so what I would do is copy the whole
[129:49] of our cell to Edge Network part and bring it down to your SSG section.
[129:52] - Okay. Copy, paste.
[130:04] - All right, get rid of that arrow. Okay, so you want like an arrow down
[130:14] from that npm build. And that's where you will say,
[130:18] render pages as HTML files or something to that effect. - Okay.
[130:39] - And then off of the Edge Network, you now have serve rendered pages
[130:43] plus JavaScript, plus CSS, plus images. - So because it does this first or during the build,
[131:01] it renders the pages as HTML files. The next step goes to the Edge Network
[131:08] and then it does the SSR stuff? - Nope, no one, it doesn't need to do SSR.
[131:16] The HTML files already exist with SSG. It's pre-created them.
[131:21] - Okay, so then it goes the Edge Network then to somebody's browser.
[131:27] - Yeah, so that's, yeah, it's gonna, the Edge Network is now gonna serve
[131:31] those HTML files directly. Doesn't have to render them,
[131:35] it can just simply serve them or send them to the user.
[131:39] - Users browser, so SSG is almost like less complicated than what's going on up here.
[131:53] - Right, that part on the SSG where it says render pages as HTML files,
[131:58] that'll do the whole contact Ivan, contact third party APIs, et cetera, and get the data.
[132:05] - Where would we put like the browser request, like the blog request?
[132:15] - You wouldn't, so what happens is you, when you're setting up SSG in Next and you know--
[132:23] - It automatically does it, 'cause it never changes. - Well, yeah, you set up, so in Next,
[132:31] you add extra functions to your route components, so like SSRs, get server side props,
[132:42] and I feel like they changed the SSG one since I last looked, but it used to be get static props,
[132:50] but I feel like they changed it, so let me just double check.
[132:55] Actually, I'm not gonna worry about it, it doesn't really matter.
[132:59] You add these functions and those are server side functions which, by existing, they say,
[133:07] oh, there's get server side props, that's gonna server side render the page.
[133:12] Oh, there's the function for SSG, that's gonna statically generate the page.
[133:17] And in those functions, you handle your request to get your data, right?
[133:27] So in that function, you would say, you would write your code to connect your database
[133:31] and query for your 10 blog posts, and then you return that queried data from that function,
[133:39] and then that data gets brought in as a prop to your actual page, and then it can use it to render it.
[133:46] - I'm gonna say okay, because what you're saying does make sense, but at the same time,
[133:57] this last part is not clicking, but we found here a lot. - Yeah, it's super important to understand
[134:02] that last part, though. So essentially, you have an extra function on your...
[134:08] So next you do, it's kind of like Astro, you have a TSX or JSX or whatever file for each route, right?
[134:17] So let's say you have your blog index one, so you have a blog.tsx file.
[134:23] And so you write your component, which is how it's gonna be displayed,
[134:27] how you're gonna create a grid of those posts or a list of those posts or whatever.
[134:31] But then separate from that, you have a function that says, hey, we're gonna render this as a static page.
[134:41] In order to do that, I need to provide these 10 blog posts as data for that process.
[134:50] So let's connect to the database, get those 10 blog posts, and have that data available to the rendering process.
[134:59] So then when you do npm run build, during that build process,
[135:05] so literally during that build process, that code will get executed.
[135:11] During the build process, you'll connect to the database and get those 10 blog posts.
[135:15] And you'll get that data. Okay, I think I just need more room to,
[135:25] and then I can put what I think you're saying. So when it's doing the build and we'll render pages as HTML,
[135:43] this is when it is going through and going to pg_admin or pg_database, any APIs.
[135:54] Apparently, what are you doing? Thank you.
[136:06] JavaScript, all of that, images. - No, well, I mean,
[136:19] it's not necessarily the images. You're gonna, it'll know the images will be there.
[136:24] There's nothing, it doesn't really do anything with the images.
[136:27] - Okay. - Like it'll just render the HTML that says,
[136:31] "Hey, get this image." But yeah, as it renders those pages,
[136:37] it'll connect to your database as needed and query the information, or a third-party API,
[136:44] like you're connecting to get the weather information on a given day or something like that, whatever it is.
[136:49] It'll make those queries, get that information, and use that information when it creates those HTML pages.
[136:56] In fact, let's use the weather example. This'll probably help to make sense, right?
[137:10] So let's say you work on your website today and you decide that you want to display the weather, right?
[137:19] So you write some code to go and get the current weather for your hometown, right, and display that.
[137:26] But then you decide to server, sorry, statically generate the page.
[137:33] So then what happens is when you take your code, you're done, you're like, "That looks good."
[137:38] You commit it to your repo, you push it up to GitHub. Vercel says, "Oh, new changes,"
[137:46] grabs a new copy of your repo from GitHub, does the npm install, npm build.
[137:53] During the build process, it says, "Oh, I'm statically generating these pages."
[137:57] So it creates those pages. During that process, it connects to the weather API
[138:01] and gets the weather for today, right, when it does it. So you're like, what's your weather?
[138:07] 10, well, no, you're Fahrenheit, so it's like, I don't know, whatever,
[138:10] 50 degrees or something like that. Sunny and 50 degrees where you're at today.
[138:15] So it statically generates these pages and it shows that weather at the time
[138:21] that it does that build step. Now, let's say I visit your page on Wednesday
[138:27] and it has gotten really cold and snowy and cloudy. Because the page was statically generated,
[138:34] I will at least initially see sunny and 50 degrees. Hydration, you know, when that JavaScript gets attached
[138:46] after initial load will probably update that depending on how you built the page,
[138:52] but you should update that. And then it should flip to the new,
[138:55] it should re-query the API live and get the new information, but it should initially at least,
[139:04] the statically generated page will have today's weather. That make sense?
[139:10] - I think so. I think I'm there.
[139:38] - Pretty sure. - I need all of this to be out of my way.
[139:44] - Sure, it works. You can go there.
[139:47] - So when something is GitHub, new commit, it goes to Vercel.
[140:07] Vercel says, okay, let me grab all the content. We'll make sure it's good because it updates all content.
[140:21] And then it's like, cool, let's do NPM install, NPM run build, and we're going to check the database
[140:29] and APIs if there's any new content. If there is, then we'll put it onto the static page.
[140:36] - So to be correct, it doesn't check for new content. It just gets the current copy of the content.
[140:45] It doesn't care whether it's new or not. It just says you want the 10 most recent blog posts.
[140:51] It doesn't, it'll still do the page, the rendering and the data request,
[140:57] whether the current build already had that. 'Cause it's building a fresh copy.
[141:04] It has no idea what was built seven days ago, right? - Okay, and?
[141:11] - It doesn't know that you have the same blog posts as seven days ago and all you did
[141:14] is change your contact page today. It just, it's a whole new build,
[141:19] and it just assumes that it needs all the information. - And that is, we'll copy the current page,
[141:27] and then it'll put it to the user's browser as a-- - Nope, so now you have all of this stuff rendered.
[141:37] It puts it on the Edge network, pre-rendered. - Pre-rendered.
[141:43] - Yep, so you already, all the HTML pages are already created.
[141:47] So now when the user visits one of your pages, the Edge network that's hosting the page says,
[141:54] oh, you want the contact page? There you go.
[141:57] You want the blog index page? There you go.
[142:00] It doesn't, the Edge network and Vercel don't need to server-side render it.
[142:04] It's already been statically generated. So it just sends that blog index,
[142:09] that HTML file with the blog index, straight to the user. - Okay.
[142:15] And then if there is like an API or something, like the weather, it's the hydration
[142:22] that's going to update the static page? - Should, yeah.
[142:26] Depending on how you set up the page, but it should update the page, yes.
[142:29] - Okay. So I get part one of like, you know,
[142:43] shared hosting and all of that. And then I get part two of like what we were saying
[142:48] that Vercel does with the SPA and SSR and SSG. But what does shared hosting do with like the VPS
[143:02] or managed WordPress? Or are those all just, like how often do they get updated?
[143:11] Or are they all just? - So most of those, so again,
[143:18] you have to remember that when you start talking about WordPress, it has nothing to do with the hosting.
[143:26] It has to do instead with what the project is. So if I want to statically generate a React website
[143:37] using Next, and then deploy that onto a VPS, I could do that.
[143:47] - Okay. - And then it would only get updated
[143:50] when I deploy it again. Right?
[143:54] - Okay. - So it depends, right?
[143:57] So this whole SPA SSR SSG, that's not specifically Next. Next is doing that, but that's not specifically Next.
[144:10] That can happen when you deploy your React application or whatever, your JavaScript application,
[144:17] your Astra application to other types of services as well. Right, so you could 100% take your Astra application,
[144:26] build your website, right? And you're like, okay, it's working perfectly.
[144:32] You do the Astra build command, which is probably npm run build,
[144:36] but I'd have to double check that off the top of my head. Actually, I'm pretty sure it's npm run build
[144:41] 'cause it's on Vite. And then Astra will build a static.
[144:47] Yeah, I thought so. As soon as I remembered it's Vite, I was like, yeah.
[144:50] Thank you though, for confirming. Astra will build static pages
[144:57] and bundle your JavaScript and your CSS. And you could then take that build
[145:02] and actually deploy it on GoDaddy via FTP on a shared hosting account.
[145:09] - But then when you make a new commit, it's not going to update.
[145:18] - It's not gonna update nearly as nicely. You would have to do the build locally again
[145:21] and you would have to FTP it, which is yes, yes, exactly. That's not fun at all, is it?
[145:26] It's much nicer to have Vercel just do it automatically. So all of these more modern tooling that we,
[145:32] or hosts that we use, Vercel, Netlify, Railway, Render, et cetera, they almost all have a step
[145:41] where they handle grabbing that information from GitHub and deploying it.
[145:47] There are ways to, so no, there are ways to integrate Git into other hosting and stuff like that.
[145:56] But usually it's not as smooth or as painless, especially the setup process.
[146:06] - Thanks, I was writing it as a note, but I like that it worked.
[146:15] - Yeah, the answer is like, if you looked at GoDaddy now, there's probably a way to have it interface
[146:23] with a GitHub account. I don't know how well that works.
[146:27] I haven't touched Git on GoDaddy or shared hosting. I haven't tried to do that kind of stuff
[146:35] for a few years now, so I don't know what the modern tooling looks like.
[146:38] When I tried it before, usually the setup was annoying and kind of getting everything working.
[146:44] - Do things like Vercel charge based on usage then or room? - Usage, yep.
[146:53] So they actually keep copies of every deployment you've ever made, I believe, or at least a lot of them.
[147:00] I've never bothered to check how far back it goes, but it certainly goes a long way back.
[147:05] But their pricing, if you go to, if you look at it, you get, you're paying for bandwidth,
[147:13] you're paying for team members who can use it, and you're paying for their serverless function requests
[147:22] and execution, which is something else to talk about, but. - Yeah, I'm like, I feel like I am tapped out
[147:33] on the knowledge side. We went through a ton, and I loved it,
[147:38] and there's so much going on right now. - So the one last thing I want to add is,
[147:43] we've mentioned this whole Edge network. So Edge network is essentially,
[147:47] the easiest way to think about it is like a CDN for Vercel. So you're taking, unlike GoDaddy's shared hosting,
[147:58] which is in one physical location, with Vercel or Netlify, you're automatically deploying
[148:05] your files to places all over the world. To quote-unquote the Edge,
[148:13] the Edge of the network near the user, is what that kind of is trying to go, like, hint at.
[148:20] So that Vercel, you know, all of that stuff, that CDN stuff, et cetera, is all taken care of for you.
[148:27] The same way they automatically take care of a free SSL server.
[148:31] You don't have to worry about that or pay for that. That stuff's all taken care of for you.
[148:35] So if you're deploying to Vercel, you're automatically deploying to a CDN.
[148:42] And your users are automatically going to have a CDN node that is close or relatively close to them.
[148:50] So that the performance will be good. And then when you deploy again,
[148:55] it will update all of those CDN nodes. So your website is, you know,
[149:02] updated across the Edge network. - Okay.
[149:08] - Like, it does make sense, but I'm like, I'm too mushy-brained right now to like--
[149:17] - Yeah, we've gone over a lot, so. - But it's so helpful because without revisiting
[149:24] what I was previously taught, like, it wouldn't have connected as well.
[149:32] So I really, really appreciate that. I will be uploading all my lovely notes
[149:38] in a more legible way later. And these are the types of things
[149:45] I'm excited about getting up and running on my website because when I have photos like these,
[149:53] it's gonna be easier just to make sure they're linked and that people can read them when they need to
[149:58] than just images, but kind of a mess and a half. We'll work through that process eventually.
[150:06] - So much knowledge. - The squares, it's definitely the squares
[150:11] that help understanding what's going on. - For sure.
[150:15] - And it also makes sense what hydration does. A lot better than I've ever understood before.
[150:26] - I remember when I was learning React, I would hear people talk about hydration
[150:29] and like, I was like, what is hydration? And then when I finally was like,
[150:35] oh, I should go understand it. I was like, oh, that's so simple to understand.
[150:39] Why didn't I Google it like five months ago? But it's a key thing.
[150:44] - It also, I feel like doesn't always make sense. At least for me, this was really helpful
[150:50] seeing the little graphics to go with it because I could understand the process
[150:55] where if it's in text format, I'm just like, you're telling me something,
[151:00] but I don't have little boxes or visuals that show me what it is.
[151:05] - Everyone learns differently, for sure. And yeah, the other thing too,
[151:10] is a lot of courses that'll teach React or whatever, they don't teach this stuff
[151:15] 'cause it's not part of the language or the framework and it's not, it's boring, right?
[151:22] A lot of courses, I see a lot of people that come out of school or come out of courses
[151:28] and they have no idea how to deploy stuff or handle deployment errors and stuff like that.
[151:33] They're like, oh, I just did npm run dev and that's all I ever had to do in my bootcamp.
[151:37] Like, how do I make it go live? And there's just not all great information on that.
[151:44] - I am laughing because you're like, yeah, it's boring and stuff.
[151:47] And I'm like, I just found this all so fascinating. But I'm also the person that--
[151:52] - Sorry, I should qualify. It's boring if you were sitting down to learn React.
[151:55] You're like, why am I learning about hosting, right? Like, I wanna learn about React.
[151:59] Make things go burr on the screen. Don't talk about hosting to me.
[152:03] - That is fair, that is fair. And thank you everyone for joining today.
[152:09] Like, we got a really dope raid. We've had people stay and hang out.
[152:13] And yeah, I stream very, very, like one to four times a week, somewhere around this time frame.
[152:25] Yet next week and the week after, I am out of town. I am going to Portugal and Munich
[152:32] and hosting Forge Nation through Vue School. So it's an online conference.
[152:41] You can see me there if you wanna come hang out that week. But we still have a few more streams this week.
[152:47] And yeah, now to go through all this. Is there anything we missed
[152:53] that you wanted to make sure we tackled today? - I mean, this is just a lot of kind of high level stuff.
[153:00] Like I said, we're simplifying a lot of it. All of this stuff is exceptionally detailed.
[153:07] So I think really the key is like, go through it, figure out what questions you still have.
[153:11] And maybe we can do a follow-up stream or at least a follow-up talk and go over them.
[153:16] I guess the only other minor thing I would add, just for anyone who's listening,
[153:19] and I think you kind of asked about it earlier, it's like pricing is like,
[153:23] why does GoDaddy charge for everything versus why do you get to get stuff free from Vercel?
[153:30] The answer with all of these tools, like Vercel, Netlify,
[153:34] Ivan just launched their free tier, PlanetScale, Railway, et cetera.
[153:40] They all have a free tier because there's a whole bunch of developers
[153:42] that are building projects and learning stuff. And if they can use these tools for free
[153:50] and get used to how good Railway is or how good Vercel is, then they'll advocate to use those when they join companies
[153:57] or if their side project becomes successful, they'll move from a free tier to a paid tier, et cetera.
[154:03] So it's a, and realistically, a lot of the stuff that gets hosted on the free tiers
[154:08] isn't very active and isn't using a lot of resources. Typically, some people try to scam the system.
[154:16] So Railway has like, they have like a free tier where you can deploy like a node app
[154:22] or whatever you want, including a database. And they recently had to change how they,
[154:29] like some of the terms on their free tier 'cause people were getting,
[154:32] I don't know the exact details, but people were getting around the database limitations
[154:38] on the free tier by recreating their database every hour so they could use, they didn't have to pay.
[154:45] So they, the free tier with Railway now means you can only create five databases a month
[154:53] so that people can't do that. But most people just are not that active,
[154:57] or I shouldn't say that, not people, their projects aren't that active.
[155:00] So you don't have to pay a lot to house all these projects, but what you do is make friends and fans
[155:07] with the developers who will hopefully all turn into, not all, but many will turn into paying customers
[155:13] down the road, and that's how they make their money. - And adding to that, I think a big reason
[155:18] why other, like it's been considered old school hosting or shared hosting has a cost is it's,
[155:27] a lot of it is done for you. Like for cPanel, they automatically set it up
[155:33] to connect to your database. So you don't have to manually do that stuff.
[155:40] At least that's my envisioning of why they would have it, but it doesn't mean--
[155:45] - Part of that too, if you think about GoDaddy is that if I knew nothing about websites,
[155:51] I'm, I don't know, I own a bakery store, and I'm like, I want to do my own website.
[155:57] I Google and I'm like, how to have my own website? And like the first result is GoDaddy,
[156:02] like create your own website without having to learn any programming for 4.99 a month.
[156:08] So I click on that and all of a sudden I end up with a WordPress website.
[156:12] I haven't had to learn programming, I haven't had to understand hosting,
[156:16] I haven't had to upload anything, I just now have a WordPress website.
[156:20] And I'm like, oh, okay, cool. And like figure it out from there, hopefully,
[156:24] or hopefully not, however GoDaddy wants to do it, 'cause they probably want to flip you on other services.
[156:30] But yeah, that's kind of how, it's like a different environment.
[156:34] Like with React, yeah, 100%. - 100%, yeah.
[156:41] - Like there's lots of people who are gonna, who run WordPress sites super successfully.
[156:45] It's not, there's no knock on that, it's just a different approach.
[156:50] No one, like there's no situation where you're like, hey, I know nothing about websites and I want to deploy it,
[156:55] and then you end up with a React website that works. Not like, not reasonably.
[157:00] Like it just doesn't, you know, you don't hit up a host and Vercel's not like,
[157:04] oh, here's your React website, and now you can just go configure it.
[157:07] Like it's two very different sides of web development. And one of the things with WordPress is that
[157:15] you can literally build an entire WordPress website with e-com and like all sorts of stuff.
[157:20] Like you can do like a learning site with courses, you can do all of this stuff,
[157:25] and never write a line of code, because all of the tools are there,
[157:29] whether it's themes, plugins, WordPress itself. Which is, you know, great for a lot of people
[157:34] and a lot of businesses. But also not great for other people.
[157:39] So, you know, that's why we have all these different options.
[157:42] - I hate WordPress personally, but that's me. You know, like I just--
[157:46] - I know how to, I know how to troubleshoot WordPress. I know how to help people once a WordPress site is developed.
[157:54] Not awesome at building it from scratch, ever. Never successfully done that.
[158:01] - Yeah. - And that's really funny to me,
[158:04] especially being part of WordCamp. And yes, so everyone, go follow Roy on Twitter.
[158:11] So, you have somewhere that you can go bug him to come back on the show.
[158:17] And also make sure that you subscribe on YouTube and follow, and if you feel so willing,
[158:26] subscribe here as well. And I will link YouTube,
[158:32] and I need to go find your Twitter, Twitter. And then--
[158:37] - @royinger, super easy. - Easy, that is easy.
[158:42] But you know, I'm still gonna go grab it to link it. And then last but not least,
[158:49] y'all, I'm gonna raid you over to Chris Griffin because I know that he's always doing
[158:57] some fun content over there. And thank you everyone for joining.
[159:02] And hit me up on Twitter, on YouTube. If you have questions,
[159:06] if you want to see us go into a specific direction. And yeah, see you later, everyone.
[159:13] - Bye. - Bye. [BLANK_AUDIO]

