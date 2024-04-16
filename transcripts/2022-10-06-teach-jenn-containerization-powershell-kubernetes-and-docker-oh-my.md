---
showLink: "https://www.youtube.com/watch?v=22R0zlOSqAw"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-containerization-powershell-kubernetes-and-docker-oh-my"
title: "Teach Jenn Containerization, #Powershell, #Kubernetes, and #Docker? OH MY!"
publishDate: "2022-10-06"
coverImage: "https://i.ytimg.com/vi/22R0zlOSqAw/maxresdefault.jpg"
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

[00:00] Just little value adds. - Yay.
[00:02] And hello, hello, beautiful humans. Thank you for joining another episode of Teach Gen Tech.
[00:09] I am excited and nervous about today's episode because I feel like this is something
[00:16] that we all are supposed to know, yet it's hard to conceptualize.
[00:19] So yay, Trevor, for joining us today. Please introduce yourself
[00:24] and what you'll be teaching us today. - Well, hello, Jen.
[00:28] Thanks for having me on your show. Great job on it, by the way.
[00:31] It looks very professional. I like what you're doing, learning lots of new technology.
[00:36] Very awesome thing to be doing, but my name is Trevor Sullivan.
[00:40] I've been in the software industry for about 18 and a half years at this point
[00:45] and held a variety of different roles, done consulting, done internal IT.
[00:50] But for the last couple of years, about two and a half years now,
[00:53] I've been working for a company called CBT Nuggets. We create software training.
[00:58] We also create IT infrastructure training. I myself have taught on a range of topics
[01:02] from AWS to PowerShell to Kubernetes certification training to MySQL database training,
[01:11] GitHub Actions automation training, and a whole bunch of fun stuff like that.
[01:14] So I'm really passionate about just helping people leverage technology,
[01:18] learning new technologies myself. That's part of the fun of it.
[01:21] And yeah, that's kind of what I do. - Curiosity, what was the first piece of tech
[01:28] that you learned? - Ooh, that's a good question.
[01:31] Well, I mean, back in my earliest IT days, back in like early 2004,
[01:36] I remember one of the earliest things that I was working with
[01:39] was this program called the Norton Ghost. And anybody who's any old timers
[01:44] are gonna laugh at me for using that software or mentioning that name,
[01:47] but Norton Ghost was the imaging product that we use to make replicas of hard drives
[01:54] to replicate desktop computers. So we'd basically make kind of a master image
[01:58] and then copy that to other computers. And that's how we would roll out
[02:02] desktop and laptop systems. - Interesting.
[02:06] I never knew that existed. - It's funny to even like talk about it.
[02:12] - What up, Anthony? Okay, interesting.
[02:18] And I know like today we're going more of the, like when do you use Kubernetes
[02:25] and when do you use Docker? And then the cool things PowerShell
[02:28] can do with Kubernetes. But when did you start working with these products?
[02:34] - Let's see, Kubernetes is relatively new to me. I mean, it's been around since I wanna say 2014 or 2015,
[02:42] at least in its very early stages when it was still initially a Google project.
[02:47] But I've only been using Kubernetes for probably less than a year at this point.
[02:52] So it's still pretty new to me. But PowerShell, I've actually been writing
[02:57] since almost since it came out, probably like three to six months after it came out in 2006,
[03:03] I've been writing PowerShell. - Okay, and hi Helmi.
[03:10] And Anthony was one of the first people on the show and has been a part of this journey.
[03:14] And he said he has a hunch that I'm not gonna need to be using Kubernetes anytime soon.
[03:22] Docker though is something I'm gonna use consistently. Well, you lead me to my next great question.
[03:30] I feel like it's a great question. What are they?
[03:33] 'Cause I've installed Docker once and I didn't know what I was doing with it.
[03:38] And I know that I have, I used to have like a ton of Docker shirts
[03:45] because a family member used to work there at one point, but this was before I knew what it was.
[03:50] And I'm kind of sad because I gave all those shirts away and I'm like, it's so cool now.
[03:54] But that is, I don't know what they are. Like I know what they are, but I don't know what they are.
[04:00] - You gave them away? - Well, it was in 20, yeah, all the shirts,
[04:06] I gave them away in 2017 probably because I didn't know what Docker was.
[04:11] It was just a cool ship, like whale thing. That's all I knew of what Docker was.
[04:20] With a bunch of containers on its back. What does that have to do with technology?
[04:24] It's all about logistics. - That's kind of what I thought.
[04:28] And so containers, before we go through like Docker and Kubernetes,
[04:34] what's a container? - So I'm probably gonna do a terrible job explaining this,
[04:38] but the way that I would describe a container is it basically, it's a level of isolation.
[04:44] So I like to kind of equate it to a virtual machine, but it's not, it's not a separate virtual machine
[04:50] where you have like a virtualized CPU and virtualized memory, virtualized disk,
[04:55] virtualized networking. But it does have its own level of isolation.
[05:00] It's just isolating at the process layer. So on your Mac OS system,
[05:04] which I believe you're on a Mac book, Jen, you run Google Chrome, you run Firefox,
[05:09] you run iTerm2, you run different applications on your computer.
[05:13] Well, each of those is a separate process or in some cases, multiple processes.
[05:18] If you look at activity monitor on your Mac, you'll actually see a bunch
[05:21] of different Chrome processes in there, probably for each tab that you have open.
[05:26] And so Docker kind of allows you to isolate programs at the process level rather than at the hardware level,
[05:33] like virtual machines do. And so containers use a few different
[05:37] underlying Linux kernel technologies, like what's known as namespaces, Linux namespaces,
[05:42] as well as C groups to control access to the underlying hardware resources.
[05:48] So what that does is it allows you to kind of isolate a process and say,
[05:52] you're only allowed to use X amount of system resources. And if you try to exceed that,
[05:56] then we're gonna basically kill you off and you can restart if you want to,
[06:01] but you're not gonna be able to exceed this particular limit.
[06:04] And so that can prevent contention for system resources and kind of do fair sharing of resources
[06:12] across a single system, or in the case of Kubernetes, across an entire cluster of resources.
[06:17] So a container is kind of a way to kind of isolate a process and kind of box it into its own little segment
[06:25] of the system and prevent it from kind of stepping on the toes of other processes.
[06:29] And that actually works at the file system level too, which is really powerful because what it lets you do
[06:34] is if you've ever tried to do, you mentioned TypeScript programming,
[06:38] or if you've ever tried to install like Python or any other runtimes,
[06:42] then you can actually run into a lot of issues when you try to install multiple versions of runtime.
[06:47] So if you try to install like Python 3.9 and Python 3.10 and Python 3.6 and Python 2.7 all at the same time,
[06:56] then these different versions of different Python runtimes can actually step on each other's toes.
[07:01] But when you use something like Docker or containers, I should say, to isolate the file system,
[07:07] then these different versions of a Python runtime or a PowerShell runtime or a Ruby runtime,
[07:12] they can't step on each other's toes. And so you don't have that in the Windows world,
[07:17] we always called it DLL hell, where you have different versions of libraries
[07:21] that are kind of mismatched with each other. And this version of Python depends on this version
[07:27] and this version of Python depends on this different version.
[07:29] And so it really avoids that dependency hell. So it just-
[07:34] - Yeah, I just went through that on Monday. - Oh. - It was fun.
[07:39] - With which runtime? - I'm thinking about it.
[07:46] Thinking about it. - Was it TypeScript? - Was it?
[07:49] No, it actually, I think it was the... Anthony, which one was it?
[07:54] - Node? - I just, we were doing a lot.
[07:56] I think it might've even been for Node. I think it was Node, so I could do the GitHub CLI.
[08:07] - Gotcha. - And yeah. So Node 18 is the newest,
[08:14] but what I was trying to clone and use was on like 18 or 16.blah, blah, blah.
[08:23] So it didn't let me do it. And then I tried just installing the lower version
[08:29] and it wouldn't let me do it because it had 18 on there. And I was gonna get my Mac back soon
[08:35] and it's having its own issues. So if I do randomly disappear while you were talking,
[08:40] my Mac just shut down all of my screens and then turned them back on.
[08:45] So I'm hoping for the best on this stream. - I can still see you.
[08:50] - Yes, okay. And then Anthony just said GitHub CLI
[08:59] is done through Homebrew probably. Oh, it was Node for Open Sauce, not for GitHub CLI.
[09:04] Okay, cool. See, this is why-- - Node for Open what?
[09:09] - Open Sauce, it's a open-sourced repo that bduggy started.
[09:16] It's actually really cool. I will put it here in the chat here shortly.
[09:19] Give me just a second. It's pretty cool because it's one of the first ones,
[09:31] like, as I'm learning to use GitHub more, like, you've talked about GitHub Actions
[09:37] and I'm really excited to hear about that later on. I've learned a little bit about it,
[09:44] but we were talking with Open Sauce on Monday because of Hacktoberfest and contributing to open source.
[09:51] So now, if I was hearing you correctly with the explanation of a container,
[10:01] I like how you mentioned it's different than a virtual machine.
[10:07] And then the, if I heard right, the container has a specific size limit?
[10:16] - Yeah, you can limit resources like CPU and memory so that it can't chew up all the CPUs on your system
[10:24] and break everything else, basically. Yeah. - Okay.
[10:27] - And that's a feature in the Linux kernel called cgroups, I believe.
[10:31] Or is it ulimits? I can't remember.
[10:34] I think it's cgroups. Yeah, cgroups allow you to allocate resources
[10:38] such as CPU time, system memory, network bandwidth, or combinations of these resources.
[10:43] So yeah, that's like a Linux kernel feature that's been implemented by container runtimes
[10:48] like Docker or Containerd. - Are there more than just Docker and Kubernetes?
[10:54] Those are like the only ones I've really heard of. - Yeah, there are actually other tools out there.
[10:59] So there's Containerd. Containerd is a runtime and Kubernetes actually shifted
[11:04] from using Docker under the covers to actually create and destroy containers
[11:09] to using Containerd relatively recently. They made that switch, I believe in one dot,
[11:15] can't remember if it was 1.24. But yeah, they switched over to using Containerd
[11:23] instead of Docker now. I guess probably due to licensing reasons
[11:27] or something like that. But then there's also Podman.
[11:31] Podman is another container tool that you can install. There's a CLI tool that you can install
[11:35] to spin up containers on your local machine. But I don't think Podman really has
[11:40] any clustering capabilities like what Kubernetes or Docker Swarm do.
[11:45] - Gotcha. I'm also Googling over here
[11:48] and I just saw Anthony's comment. These used to be a full-on industry-wide war
[11:53] over Kubernetes versus alternatives and Kubernetes ritually slaughtered all the competition.
[12:00] Oh, damn. Okay.
[12:03] - Very true. In fact, I remember attending DockerCon
[12:05] where I met your family member back in, I think, 2016. And there was a pretty big war going on
[12:14] between Apache Mesosphere, I think was another project. And then there were some other orchestrators out there.
[12:21] I can't even remember what they were called, but yeah, that does ring a bell.
[12:24] There was a little competition. - Interesting.
[12:28] Okay. - You don't really hear about them anymore.
[12:31] - Yeah. And containers like Docker is what I just Googled
[12:35] and it is coming up with quite a few other ones as well as is Kubernetes the same as Docker?
[12:44] And it definitely supported what you were just saying, like Docker is like a single container
[12:52] and Kubernetes is a system for operating containerized applications at scale.
[12:59] The words make sense. And I take that as like Docker is like...
[13:06] I was actually showing... My friend is not technical whatsoever.
[13:10] So I'm trying to like show her what I'm talking about today. And this was my explanation.
[13:15] I'm gonna use it with pens. Pens, they're fun.
[13:19] So this is like Docker and you can have like separate containers at Docker,
[13:25] but none of them are gonna go together. Where Kubernetes is like, they're all together.
[13:30] And if I remember right, if one fails, one of the other containers will help it.
[13:37] Is that accurate? - You can load balance network traffic across containers
[13:44] for sure in Kubernetes. That's actually a big value of Kubernetes
[13:48] is its load balancing capabilities. So yeah, if one pod fails,
[13:52] then another application pod can kind of take over and serve requests for that application.
[13:57] We generally refer to that as high availability. So rather than just having a single instance
[14:03] of an application that could fail and cause an outage for all of the users
[14:08] of that application, we could have 10 instances of that application.
[14:12] And then when a user tries to hit that application, they get routed to one of those 10 instances
[14:18] of the application. And we refer to that as kind of load balancing traffic
[14:22] across multiple instances of the app. So that could be a database server
[14:28] that you're doing load balancing across. You could have a client application
[14:32] that's hitting different instances of a database server. If you have replicas of a database,
[14:37] you could also have it be a web application. So if you have a web application,
[14:41] maybe you have three or four containers running that same exact code.
[14:45] And then when a user tries to go to teachgentech.com, they hit maybe container number one,
[14:51] and then another user comes in and they hit container number four,
[14:54] and then another user comes in, they hit container number two.
[14:57] So yeah, load balancing and high availability is a big value of using Kubernetes for sure.
[15:03] - And okay, that's starting to make a lot of sense. And I liked what Anthony added in,
[15:09] like Kubernetes is like a bunch of Docker containers speaking to each other.
[15:15] And so I guess that really does lead to like the next question of
[15:21] what would you use a Docker container for and what would you use Kubernetes for?
[15:26] Like, I think that's the other piece, like learning what they do,
[15:30] but having like a real life example of what they do. - So in the real world, Docker, generally speaking,
[15:39] I would say is used more as a local development tool. So if you do wanna install Docker on your MacBook,
[15:45] or if I wanna install Docker on my Windows machine, or maybe install it on a Linux host somewhere,
[15:50] I can use the Docker CLI to kind of manage containers on each of those systems individually.
[15:55] Now Docker does have a clustering mode where I can create a cluster of Linux virtual machines
[16:02] and join them all together into what's known as a swarm cluster,
[16:05] which has a little bit of overlap with Kubernetes. But when it comes to clustering capabilities,
[16:12] Kubernetes is much more powerful, I would say, than Docker swarm.
[16:18] If your needs are very basic for clustering, then a Docker swarm cluster might be enough,
[16:22] but Kubernetes is really where the industry is headed for kind of large scale container management.
[16:29] So the reason that you would use Kubernetes is if you're deploying production grade applications
[16:34] that you need to deploy in the cloud and have shared access to.
[16:38] So Kubernetes has shared a permissions model called role-based access control
[16:43] that allows multiple users to have permission to manage different resources.
[16:48] Kubernetes also has this logical concept called a namespace. It's not the same as a kernel namespace.
[16:54] So there's some ambiguity that you kind of have to get familiar with.
[16:57] So there's Linux kernel namespaces, which is a feature that containers use,
[17:01] but then Kubernetes itself has this concept called a namespace,
[17:05] which is also a term used in software development, but it basically just allows you
[17:09] to kind of carve out a piece of the cluster and say, okay, you, Jen, have access to this namespace.
[17:14] Trevor, you have access to this namespace over here. And any resources that I create in Kubernetes
[17:21] in each of those namespaces is going to be permissioned based on who has access to each of those namespaces.
[17:27] So that's a capability that exists in Kubernetes, but does not exist in Docker swarm.
[17:33] So that kind of is why I'm suggesting that Kubernetes is more used for production grade deployments,
[17:39] whereas Docker is used, generally speaking, more for kind of localized one-off containerizations.
[17:46] - Anthony said he doesn't know if he should run Docker containers in prod all the time now
[17:55] 'cause so many services have been made really easy. - I mean, you certainly can use Docker in production.
[18:02] There's nothing preventing you from doing that. It just kind of goes back to things
[18:07] like the load balancing capabilities of Kubernetes that make it a lot more powerful,
[18:11] a lot more, I guess, robust, I would say. But I mean, there's nothing preventing you
[18:17] from spinning up a Docker swarm cluster and running multiple containers,
[18:20] doing load balancing on Docker swarm. I know it supports that.
[18:24] But again, Kubernetes is just a much more flexible solution. So if you need to add on kind of bolt-on capabilities
[18:34] in Kubernetes, which you pretty much have to to make it really useful,
[18:38] it's just gonna give you a lot more capabilities than what Docker swarm would.
[18:42] - Okay, and I know like my first intro to Kubernetes was really through Denver Startup Week.
[18:53] And there was a company that came to present and they basically will help a business launch their cluster
[19:06] with all the applications that they need for it. And I think just like where my head goes with that
[19:13] is would you ever put those same type of applications in a Docker container?
[19:19] And then also like, how do you choose between all of the options in Kubernetes?
[19:28] - So if I understand your question correctly, you're asking how do I determine if I should
[19:36] or shouldn't run an application in a container? - Yes, that's a good way of saying it.
[19:43] - Just wanted to make sure I understood that properly. So containers are generally used
[19:50] for server side applications. So this is things like web servers, database servers,
[19:54] background processing tasks. So if you think about a platform like YouTube,
[19:59] for example, right? If you go to YouTube and you record a video,
[20:03] you upload that video to YouTube and then YouTube does some backend processing on your video
[20:08] before they actually publish it, right? That shows you right in the YouTube studio there
[20:12] that it's running some processing tasks and it takes a while for that to happen
[20:16] depending on how long your video is or things like that. But those kind of background processing tasks
[20:21] could be theoretically running containers. Obviously, I don't know how YouTube
[20:24] has implemented that functionality, but I'd be very surprised if they were not using containers
[20:29] on the backend to process those videos with some utility like FFmpeg, for example,
[20:35] which is a Swiss army knife utility to process videos into different formats.
[20:39] But my point is, is that generally speaking, containers are used for kind of server side applications
[20:48] that are running on the backend. Now there are some advanced ways
[20:51] that you can actually run graphical applications like Firefox or Chrome or draw.io,
[20:57] which I just kind of, we were talking about prior to launching the live stream.
[21:01] You can technically run a graphical application inside of a container,
[21:04] and then you can connect an X server to that application that's running in the container.
[21:09] So you can achieve the benefits of isolation of applications that are graphical in containers,
[21:17] but that's a little bit more of an advanced use case. And it's not generally speaking,
[21:21] what people are doing with container based applications. So generally speaking,
[21:25] you wouldn't really want to run Firefox in a container because if you download a file with Firefox
[21:30] and you download it inside of the container, well, now that file exists
[21:33] inside of the container's file system, and you on your Mac desktop need to have access
[21:38] to whatever that file is that you downloaded. So you'd have to go into the container to get the file,
[21:42] and that just kind of complicates things, but it is possible technically to do those kinds of things.
[21:48] - All right, so I think I'm starting to see it all, but where do we get started
[21:54] in getting Kubernetes or Docker? And we got a question from Rivet.
[22:03] "Why is it better or is it better to run backend "on a Docker container, Kubernetes cluster,
[22:10] "instead of say of EC2 instance?" - So an EC2 instance is basically
[22:16] just AWS's terminology for a virtual machine. So you can spin up a Linux virtual machine anywhere,
[22:22] you can use AWS, you can use Azure, you can use Google Cloud, you can use Linode,
[22:26] you can use DigitalOcean. You can even spin up virtual machines running Linux locally
[22:31] on your dev desktop using things like VMware Workstation or VirtualBox or other hypervisors like that.
[22:38] So basically, I think what the question is kind of boiling down to though
[22:43] is like why would I want to run a container-based application on,
[22:48] let's say a managed Kubernetes service rather than like self-managing a virtual machine?
[22:53] So you as a developer can go out to a cloud platform like AWS, you can spin up a Linux virtual machine,
[23:00] you can install Kubernetes on that virtual machine, and that's what we would consider
[23:03] to be a self-managed cluster. But you can also go out to these cloud providers
[23:08] and all the cloud providers that I just mentioned all provide managed Kubernetes distributions.
[23:14] So you can basically go out to the cloud provider and instead of saying create a Linux virtual machine,
[23:19] you can say create a Kubernetes cluster. And so rather than using SSH
[23:24] to go into that Linux virtual machine and installing Kubernetes yourself,
[23:28] you're basically just spinning up a pre-built Kubernetes cluster from that cloud provider,
[23:33] and then you're able to use kubectl, which is kind of your client utility to manage Kubernetes,
[23:39] to talk directly to this managed cluster rather than having to self-install
[23:44] and self-manage that cluster. So I think that's kind of where
[23:48] that question was going towards. And it's kind of a loaded question
[23:53] because there's not a right answer for anybody. Some people might be able to get away
[23:59] with using a managed Kubernetes distribution. However, when you use a managed Kubernetes distribution
[24:05] from a cloud provider, it does prevent you from configuring certain backend components of Kubernetes
[24:11] like the API server, the controller manager, and the scheduler.
[24:15] Those are kind of the three critical components of the Kubernetes master nodes.
[24:20] And when you use one of these managed cloud distributions of Kubernetes,
[24:24] they prevent you from configuring those components. They manage all that stuff for you.
[24:29] So if you have an advanced use case where you do need to configure
[24:33] some of those backend Kubernetes master node components, then a cloud-managed distribution of Kubernetes
[24:40] would not be right for you. Instead, you'd wanna look to a self-managed distribution
[24:45] of Kubernetes. - Rivet, did that help?
[24:49] And in the meantime, Homi said before he understood that to think Docker containers as a mini PC
[24:59] that only does one thing in one process. Kubernetes is a computer that joins controls
[25:06] as a bunch of mini PCs, very general. - Yeah. - All right.
[25:12] - Any way you wanna think about it that makes it easier for you is totally fine.
[25:16] But yeah, I mean, that's not a bad way to think about it. - I was like, I was going with pens earlier.
[25:23] It was when I was explaining it to my friend, it was spices.
[25:27] So maybe a better wording is why a container versus a VM. Great question. - So that is
[25:38] a very good question. So as far as containers versus virtual machine go,
[25:43] containers do not spin up a virtual machine. There is no separate kernel.
[25:48] Like there's no operating system kernel that gets spun up for each container that gets created.
[25:54] Rather, when you create a container using Docker or ContainerD or Podman or whatever,
[26:00] then what happens is that these namespaces get created inside of the Linux kernel.
[26:05] And each process can only see certain parts of the system based on what's exposed to it
[26:11] through these kernel namespaces. So rather than having,
[26:16] like in a full virtual machine environment, like if I create an EC2 instance on AWS,
[26:20] or if I create a Linux virtual machine on DigitalOcean, that's giving me an entire virtual machine
[26:26] with its own separate Linux kernel. And I can install different versions of the kernel.
[26:31] I can load modules into the kernel if I want to, because I control that kernel.
[26:36] But if I create a container, I don't have my own separate kernel that I can manage.
[26:40] It's actually a process level of isolation that's happening. So in terms of why you would want one versus the other,
[26:49] it kind of boils back to why would you want a single physical server
[26:56] that I can create multiple virtual machines on, right? Because you get better density,
[27:00] you get better, more efficient utilization of that single physical server
[27:05] by creating 10 or 20 or 30 virtual machines on that single physical server, right?
[27:10] Because if I take a single physical server and I install an operating system on it,
[27:14] and then I run just one application on that physical server, I'm probably wasting 95 to 99% of that server's capacity,
[27:22] because unless you're running some really heavy application, you're probably not gonna be utilizing all the CPUs
[27:27] and all the memory and all the disk of that server. So the way that we achieve better efficiency
[27:33] is by running additional virtual machines on the same physical server.
[27:37] Well, apply that same concept of density and efficiency to the process level.
[27:43] If I spin up a Linux virtual machine, but I only install one application on it,
[27:48] then I'm probably wasting 99% of the resources of that single Linux virtual machine.
[27:54] So what I can do is I can spin up more applications on the same server, on the same Linux instance,
[28:00] and I'm getting better efficient utilization of the resources on that system,
[28:04] rather than just wasting 99% of its capabilities. (indistinct)
[28:10] In theory, it's starting to make sense, but I feel like this is all of tech of like,
[28:15] it makes sense, but then it's also very, very confusing at the same time.
[28:19] And I don't know, I didn't know that this happens before, you know, starting Teach Gen Tech a few months ago.
[28:26] So, I think just like picking back, piggybacking off of what Rivet said of,
[28:36] and I'm glad that it helped Rivet. Yay!
[28:41] Would be something of how, words Jen, how do we go about like,
[28:53] I've seen a bit about like installing virtual machines and that kind of thing.
[28:57] Now yet, using Docker Kubernetes is very different. And you and I talked about pre-show a bit about
[29:06] doing, and if I'm paraphrasing this properly, it's like doing a local install of Kubernetes
[29:12] or using a cloud Kubernetes. First question, is Docker the same where you can do
[29:18] a local versus a cloud? And for both, when would we use them?
[29:24] And can we go through those examples? - You mean, yeah, certainly we can go through those examples.
[29:29] Generally speaking, Docker does not, most cloud providers don't provide like a managed
[29:37] Docker swarm cluster type of thing, like they do with Kubernetes.
[29:41] The cloud industry has kind of standardized on Kubernetes as a container orchestrator.
[29:45] So that's why if you go to AWS or Google Cloud, you're not gonna see an option in their cloud platform
[29:51] in their portfolio of services to like create a Docker swarm cluster.
[29:56] Now you can create your own Linux virtual machines and then you can install Docker on all of them
[30:01] and run the commands to create a swarm cluster and then join all those machines to a swarm cluster.
[30:07] But those cloud providers are not gonna provide that same kind of managed service for a Docker swarm cluster
[30:13] like they do with Kubernetes. But you can install Docker on a virtual machine.
[30:19] You can install Kubernetes on a virtual machine. If you control the virtual machine itself
[30:25] or multiple virtual machines, then you can create your own clusters,
[30:29] configure your own clusters. However you want to.
[30:33] Now, one of the things that we had talked about a couple of days ago, or I guess last week,
[30:36] maybe when we initially got in touch was that there's a bunch of different Kubernetes
[30:41] distributions out there. So if you do want to run Kubernetes yourself
[30:44] on your own Linux virtual machine, like on your laptop or on my Windows 11
[30:49] developer workstation here, if I want to install Kubernetes on my own
[30:52] local Linux virtual machines, there's a lot of different Kubernetes distributions
[30:57] and tools that you can use to actually instantiate a Kubernetes cluster.
[31:01] My personal favorite that I actually use in a lot of my training for CBT Nuggets on Kubernetes
[31:07] is called K3S. So if you go to k3s.io,
[31:11] it's a very well-supported distribution of Kubernetes from Rancher Labs that allows you
[31:18] to rapidly spin up a cluster. It's just a single binary.
[31:21] So you literally just download K3S itself and then it contains all the different components
[31:25] of Kubernetes. And it also gives you a lot of control
[31:28] over passing in different configuration options to each of those components that I discussed previously,
[31:34] the Kubernetes scheduler, the API server, and the controller manager.
[31:39] And so you can customize, you know, like the logging paths,
[31:43] like where to spit out log files. You can enable audit logging on the API server
[31:47] if you want to, which is a little bit more of an advanced security feature.
[31:51] And it gives you just that full control, but it also gives you that simplicity
[31:55] because it is just so easy to spin up a cluster. But if you want to,
[32:00] you could also use more official utilities. Like the official utility to create a cluster
[32:04] is pretty complicated. So I wouldn't recommend it to newbies,
[32:07] but it's called kubeadm, short for I think kubeadministrator or something like that.
[32:11] But it's basically the command line tool that you use officially from the Kubernetes project
[32:16] to create and configure a cluster of Kubernetes nodes. Much harder to use,
[32:23] but it also does give you a lot more flexibility and it is also the official tool from the Kubernetes team.
[32:29] So that's kind of like the best way to go if you're looking for the most raw experience.
[32:34] - I'm letting that soak in because, so it's the k3s.io, I believe.
[32:44] I'm taking a look there just to see if, they also have a very, very bright website.
[32:52] I think my screen will let me make friends. We'll find out.
[32:57] Give me just a second and we'll see if my computer, okay, cool.
[33:06] So I'm taking a look at it and I feel like Ben, he's not here,
[33:13] but he makes me think about accessibility and doing the contrast.
[33:23] And I'm like, I can barely read the white on the yellow. And it's so funny.
[33:28] He's like always in the back of my head. So, okay, cool.
[33:32] You run this and you got it. - It's literally that easy.
[33:38] - Cool. So we got that going for us.
[33:40] I'm not gonna do it just yet, but this is like one place we could start.
[33:45] Or you said that we could start with DigitalOcean, right? - So DigitalOcean is kind of,
[33:55] I always like to think in the cloud world, there's like the big three cloud vendors,
[33:58] Microsoft Azure, Amazon Web Services, and Google Cloud Platform, GCP.
[34:05] But then there's a lot of smaller cloud vendors out there. DigitalOcean is one of those.
[34:09] They're actually a publicly traded corporation. So they are pretty large.
[34:12] But then there's also some others like Linode. I use Linode pretty heavily.
[34:16] And these smaller cloud providers have a lot of benefits. Number one is they're easy to use
[34:21] because they don't have the massive portfolio of services that some of the major cloud vendors have.
[34:26] So it's a lot more straightforward of a platform to use for people who are new to cloud.
[34:31] And also their pricing, one of the things I love about them
[34:35] is that their pricing is a lot more straightforward. If you get deep into the pricing of the major cloud vendors,
[34:41] especially like Amazon Web Services, their pricing is so complicated to figure out
[34:46] that it can really cause your head to kind of spin. So what I like about DigitalOcean
[34:51] or Linode for that matter, or Vulture, is that they have simple platforms.
[34:56] It's like, here's your virtual machine infrastructure, here's your Kubernetes clusters,
[34:59] here's your managed databases, but that's it. And their pricing is very straightforward.
[35:05] It's very competitive pricing as well. So they're not trying to screw you over.
[35:10] It's actually a very pleasant experience. - Yeah, and I totally didn't set this up beforehand
[35:15] to do the account. So do you have one on DigitalOcean that we could check out?
[35:22] - Yeah, I spun up one actually on the Linode platform. So if you wanna share my screen,
[35:28] you're more than welcome to. - Sweet.
[35:30] - So I've created a Linux virtual machine here. It just has two CPU cores and four gigabytes of memory
[35:38] and a little bit of storage here. It's plenty for doing a basic cluster here.
[35:43] It just gives you a public IP address here. And then you associate an SSH key
[35:47] just to authenticate to the cluster. So I can connect to this cluster from any machine.
[35:53] I could do it from Jen's machine if I wanted to, I could do it from my Windows machine here,
[35:59] or I could, if I was running Linux locally, obviously every operating system these days
[36:03] has SSH built into it. So if I just run SSH root at IP address,
[36:10] I should get automatically logged in here once I confirm the host key.
[36:13] And boom, now I have my own Linux virtual machine running up in the cloud.
[36:19] And if I wanted to, I could destroy that Linux virtual machine,
[36:21] create a brand new one, start from scratch again, and I'm good to go.
[36:25] Now the Linux distribution that I have installed on this machine, so when I created this Linode machine here,
[36:32] I chose the Ubuntu Linux distribution, which is extremely popular.
[36:38] It's from Canonical. They make awesome software.
[36:41] Ubuntu has been around for a very long time. I typically use the LTS, the long-term support version of it
[36:46] just because it's more stable than the interim releases that they have.
[36:52] So like these 21.10, 21.04, those are kind of interim releases of Ubuntu Linux.
[36:59] So I tend to stick with the long-term support versions of it just for that stability.
[37:03] But there are, as you probably know, tons of Linux distributions out there.
[37:06] Debian Linux is actually what Ubuntu is based on. So if you want a more core Debian experience,
[37:12] you can just use that. You can use Fedora Linux if you want to,
[37:16] and a bunch of other ones out there. But I typically just stick with Ubuntu.
[37:21] And so I've got Ubuntu Linux running on this machine here. If I run this uname -a command,
[37:26] or actually let me do lsb release --all, you can see I am running Ubuntu 22.04 here.
[37:35] So this command here is what I can use to kind of verify which distribution of Ubuntu
[37:41] I'm running here. So at this point, I've got a Linux virtual machine,
[37:44] and I can do whatever I want with it. I could install Docker on it.
[37:47] I could install Kubernetes. I could use Podman, like we talked about, Containerd.
[37:53] It's really up to you what you want to do with this machine. - What are some examples
[37:58] of what someone might put on the machine? Is there something we can look up or put on there
[38:05] that is a project that someone may be working on or an application someone may be working on
[38:10] to see how that's installed? - Oh my gosh, there are tons of applications out there
[38:15] that you could spin up. Trying to think of some.
[38:18] For example, like Neo4j, have you heard of Neo4jgen? - No.
[38:25] - So Neo4j is freaking awesome. Actually, it's this concept known as a graph database engine
[38:34] where you have these nodes that represent things and then relationships, which are just lines
[38:39] that represent a relationship between two different things. So graph databases are really cool
[38:45] just because they're so simple to understand for humans. Just because our world is kind of based on graphs,
[38:51] it's like you have, on a map, you have different addresses. Those are places, right?
[38:55] We have businesses. Those are things.
[38:56] Those are nodes. Then we have relationships, like Jen visited Starbucks
[39:00] or Trevor visited his house or whatever. And so graph databases are a really nice way
[39:07] to think about data in the real world. Neo4j is a company that creates their product,
[39:14] which is Neo4j. And Neo4j is a graph database engine
[39:18] that you can deploy very easily inside of containers. And one of the nice things about Neo4j
[39:23] is that it has a web interface that you can log into to actually create data in your own graph database
[39:30] and query data from your graph database once you've inserted it.
[39:33] So one of the things I like to kind of play around with sometimes is Neo4j.
[39:38] And so if we wanted to install Neo4j, one of the easiest ways to do that
[39:42] would be to install the Docker runtime on our Linux VM and then just spin up a container using Docker
[39:49] that runs this Neo4j application. So if we head out to, do you want to do that now?
[39:55] - Sure. - Okay.
[39:57] So if we head out to the Docker hub, this is kind of a container registry
[40:01] that allows us to find different applications. And so if you search for Neo4j or search for MySQL,
[40:09] which is a relational database engine, or if I search for AppRite,
[40:15] which is this like low code runtime, that's really interesting.
[40:20] I mean, there's just so many different applications out here that are just pre-packaged as container images.
[40:25] But anyways, we've got this official Neo4j image here, and we can very easily spin up an instance of Neo4j
[40:33] by using this command right down here. But of course we need to have Docker installed first
[40:38] on this VM. So because I'm on Ubuntu Linux here,
[40:43] Ubuntu Linux has a package manager that you use to install different software packages
[40:47] called apt. So I can just run apt and then update here,
[40:51] and this will just grab some metadata about all the different packages that are available.
[40:56] I'm not actually installing anything here, but it's just gonna grab some metadata
[41:00] for the apt package manager. And then I can run apt install docker.io,
[41:05] and docker.io is the name of the package to install the Docker engine just locally
[41:11] on this Linux VM here. And once I've got the Docker package installed,
[41:15] I can immediately start spinning up containers, or if you wanted to go down the route
[41:20] of spinning up a Docker swarm cluster, I could actually create additional Linux VMs
[41:25] and then kind of combine them all into a single Docker swarm cluster.
[41:29] But as we kind of talked about before, using Docker locally is one of the more common
[41:34] use cases of it. I guess I'll kind of pause there
[41:38] and see if you wanna interject, Jen. - No, I think it's at a point where like there is,
[41:44] a lot of it is going over my head, but I'm still like absorbing it in the fact of
[41:50] piecing it all together with context, but also learning where I may dig in later on
[41:59] and ask questions. So I say at the moment, continue,
[42:04] 'cause I'm following along. It's just like, if somebody were to ask me about it,
[42:08] I'd be like, oh, but it's sticking enough conceptually.
[42:14] - Well, once you do it a few times yourself, you're gonna keep going.
[42:17] You're gonna create a few containers and you're gonna be like, oh my gosh,
[42:20] I wanna spin up this application or that application. And I've actually been documenting a bunch of,
[42:26] are you familiar with the awesome repositories out there on GitHub?
[42:29] Like awesome machine learning or awesome databases or anything like that?
[42:34] - No, but I feel like I definitely should. - I mean, there's a bunch of different repos out there.
[42:39] If you just search for like awesome GitHub, I don't know, databases,
[42:43] like people create these lists basically of like awesome database engines, right?
[42:50] And sometimes they're not always up to date. Like this one's kind of outdated by a couple of years here,
[42:54] but there's just these huge lists of different awesome topics.
[42:58] Anyways, I wanted to have control of my own list so that I didn't have to like wait for somebody
[43:03] to merge my suggestions. I created this awesome Trevor repository here
[43:08] and I've listed out just a ton of different software packages.
[43:10] Some of them are like libraries that you can load into programming languages,
[43:14] like down here towards the bottom, like PowerShell modules or .NET modules
[43:20] or JavaScript modules for different purposes. But then I've also got like a bunch of applications
[43:25] that you can install oftentimes using Docker here, like database engines, for example,
[43:32] like Neo4j is right there or RethinkDB or InfluxDB, which is another one of my favorites.
[43:38] I don't know why I didn't think of that earlier 'cause I love InfluxDB.
[43:41] It's a time series database engine for like metrics storage. Where was I going with this?
[43:47] I'm not 100%, but I just saw Ramon's question of wait, what's a swarm cluster?
[43:53] And I think a swarm cluster is where Docker can link multiple containers together.
[44:01] Kind of like Kubernetes, but it does it with Docker and they call it a swarm cluster.
[44:06] - Yep, you spin up a bunch of Linux VMs and you mash them all together inside of a single cluster.
[44:13] And then when you create a container, that container could get created
[44:17] on any one of those nodes in the cluster. And it's actually like really, really easy to set up.
[44:21] It only takes like a minute. - Okay.
[44:25] - Anyways, these are a bunch of different applications that you can like learn about for different purposes.
[44:32] But Neo4j is in there. Anyways, I think I was getting off on kind of a tangent
[44:38] there, I don't know why I mentioned that, but. - The awesome Trevor project.
[44:45] - That's just where I document a bunch of cool software, like mostly open source that I come across.
[44:49] If you're looking for like container tools, I don't know why I haven't put Podman is not in here yet.
[44:55] But if you're looking for like Kubernetes stuff, I have a bunch of like Kubernetes things down here
[45:01] for different purposes. So yeah, just kind of my personal documentation repository.
[45:08] - And I believe Ramon, I think you said that you do some of this kind of stuff at work.
[45:16] Is there any questions that you have that you'd be curious about other than the cluster one
[45:24] or the swarm cluster? And yes, bye Anthony, have a wonderful day.
[45:31] 'Cause I know we've covered quite a bit today. And I have so many things that I'm gonna end up asking
[45:42] about later on after I let it noodle for a bit. What are some resources you would suggest
[45:52] for newbies to use? Would you just say like going to Linode
[45:58] and using their docs or is there something else that like you have the training that you do
[46:05] with certifications as well, right? - Yeah, I built a lot of certification
[46:10] and kind of what I consider like practical training, like here's what you need to know to get certified,
[46:16] but then like what are the things, certifications don't always cover all scenarios, right?
[46:21] They kind of focus on very specific topics. So in the case of like AWS training,
[46:27] they're only gonna test you on like AWS stuff, right? They're not gonna necessarily test you
[46:31] on kind of all this other software that you need to know about as a developer.
[46:34] And so a lot of the training that I build, I try to think of like, what are the tools
[46:38] that people actually use in real life and build training around those types of topics,
[46:43] like GitHub Actions, for example. There is no GitHub Actions certification that I know of,
[46:48] but I still build training on GitHub Actions because that's a tool that people use in real life.
[46:53] Very powerful. - I mean, I think that,
[46:57] and I know that we've been talking very high level today and mostly through theory,
[47:03] but something that we talked about offline was like how PowerShell can help with a lot of this content.
[47:11] And now learning a bit more about it, would it mainly only help with things in Kubernetes
[47:19] or could it help with things in Docker as well? - Well, talk about opening up a can of worms.
[47:27] I could talk about PowerShell for months. Like I mentioned, I mean,
[47:31] I've been doing PowerShell since 2006 when it came out. And so PowerShell is a cross-platform.
[47:37] A lot of people still don't realize this, but in 2016, so now six years ago,
[47:42] Microsoft open-sourced PowerShell and made it a cross-platform automation language.
[47:47] So all the same types of things that you would do with Python or Ruby
[47:51] or Java programming languages, pretty much you can do with PowerShell.
[47:57] So it's an automation language that allows you to plug into lots of different platforms.
[48:02] You can use it to call REST APIs, to do cloud provisioning. You can use PowerShell like with bash scripts,
[48:08] where you're just call out to different executables to run different CLI commands in succession.
[48:14] If you want to, PowerShell does support multi-threading too. So if you want to spin up multiple parallel instances
[48:21] of work that need to be done, you can use PowerShell to accomplish that as well.
[48:26] But it's really just a general purpose programming language that you can use to write scripts.
[48:32] And you can also use PowerShell interactively to just run like one-off commands,
[48:36] like delete this file or create this file or whatever you need to do.
[48:41] So it works great for both of those. And you may have noticed I actually use PowerShell
[48:46] here on my local machine as my primary shell. Sorry, my machine's being kind of slow here.
[48:53] But yeah, I just use PowerShell locally here to run commands like get child item
[48:58] to list files on my file system. Or if I go to my git directory here,
[49:04] take a look at some of the different folders I've created. So I can use this to run various commands.
[49:09] I could run DigitalOcean commands. I could run Kubernetes commands with kubectl.
[49:15] So PowerShell works great for that interactive use, but it also works great to do like actual scripting,
[49:22] programming type of tasks too. I'm letting it set in 'cause I think at this point,
[49:29] I'm like, this is, my brain hurts. And the fact, because it is a lot to go through,
[49:37] but also working on putting it into real life action. And I think that's something that I'm struggling with.
[49:49] But I mean, I do that on everything of like, when would I actually use this?
[49:54] And in my own processes, but I, at least the way when you said PowerShell,
[50:02] the first thing I was thinking was in Python, being able to program lights.
[50:08] And I'm like, oh, so can you program lights with PowerShell? That's where my mind went.
[50:14] But I think just also this gave me a lot of thoughts around specific questions I would have here.
[50:24] Like I need a noodle on it to like figure out what the questions fully are,
[50:28] but this high level overview was really helpful to get an idea, then dig into each of them very separately.
[50:36] So I greatly appreciate that. And is there anything that you think
[50:45] we needed to cover today that we haven't? - Not really.
[50:51] I mean, it's just, you got to spend time kind of hands-on with the technology.
[50:55] I always encourage people, get hands-on time with it because the more hands-on time you spend
[50:59] with the technology, the more it's going to make sense, the more it's going to kind of jostle your mind
[51:04] and think about all the possibilities of things you could build.
[51:07] So like the other day you learned about TypeScript. It's like, okay, well, I can use TypeScript
[51:10] to build web applications. Okay, what kind of application would I want to build?
[51:16] Do I want to build Jen's to-do tracker so I can track all my work that I need to do?
[51:20] Do I want to build a dealership's car inventory tracker so that I can help a car dealership,
[51:29] track inventory and sell cars? I mean, just think of different use cases
[51:32] for what you want to do and then go out and try to build it. And as you run into challenges,
[51:38] that's going to prompt you for solving very specific problems.
[51:42] It's like, how do I use TypeScript to connect to a database? Okay, let's go research that.
[51:46] Okay, how do I use TypeScript to build a front end to a web application or build an API backend?
[51:53] Okay, I'm going to go research that topic. So the more purpose-driven that you can be
[51:57] about doing your research and the more experimentation that you do,
[52:01] the better your development journey is going to be and the less abstract things are going to feel.
[52:06] - Yeah. - 'Cause, yeah. - And I appreciate that because I feel like
[52:11] one thing that I've enjoyed about the show is being able to learn about it abstractly
[52:16] to at least kind of understand where I would, for your example, like creating,
[52:24] using TypeScript to create a to-do list. Like learning about it abstractly
[52:28] will then kind of give me ideas of where to go with it instead of just not knowing what it did altogether.
[52:35] And to the beautiful humans watching today, and I saw that Ramon also had to go.
[52:41] So bye, Ramon. You didn't see that, but bye, Ramon.
[52:44] Anyone else have any questions before we end our stream today?
[52:51] Rivet, I know if you're still here, you had good questions earlier.
[52:55] So please let us know if you have any questions or hit us both up on the Twitters
[53:01] and that's our like names there. Give you guys just a minute.
[53:09] And yeah, it's definitely a lot, but it's like a good amount of a lot.
[53:15] I think I would, like, it's hard to explain. Ooh.
[53:20] - I get excited about all sorts of technology. So, I mean, I get it.
[53:23] - Homie said if he used Next.js in Docker, that would you lose some of the Next.js features
[53:35] as opposed to deploying it on Vercel? - You know, Next.js is a really powerful framework
[53:42] and I really like Next.js. I'm not an expert with it by any stretch of the imagination,
[53:46] but I'm not familiar enough with the Vercel platform to know if they have special integrations with Next.js
[53:56] that you would lose if you spun it up on Docker or just installed it directly on a Linux VM
[54:01] without using containers. I do know that using Next.js as a web framework
[54:06] and API framework to build applications is extremely powerful regardless of where you run it,
[54:12] but I don't know enough about the Vercel platform specifically to say if you would lose functionality.
[54:20] - That's a curious question, Homie, and I appreciate it because I know Vercel created Next.js, right?
[54:29] So I'm curious too if it, without using Vercel, if it would cause issues.
[54:37] We should try to get-- - I think the way that I would approach--
[54:39] - Oh, go ahead. - I was just gonna say,
[54:42] the way that I would approach that question is think about what functionality do you need?
[54:46] So like start by developing Next.js locally, right? That's typically where you start with building applications.
[54:51] So start building your application locally and then if there's a feature that you think you're missing,
[54:56] then go research that and see if it's specific to Vercel, but personally, anytime that I find a platform
[55:03] that's gonna add some special feature that's not available in other platforms,
[55:08] I tend to shy away from that because I don't like to get locked into a platform.
[55:12] Like I wanna use Next.js to build an app, but I don't wanna be locked into just deploying it on Vercel.
[55:19] I wanna deploy it on DigitalOcean or Linode or AWS or Azure or something like that.
[55:24] I wanna have that flexibility and choice. So anytime that you find something
[55:28] that kinda locks you into a specific direction, that's usually a red flag to me
[55:33] and I probably would not personally want to take a dependency on whatever that feature is.
[55:39] - Homie, I feel like we need to tweet them and ask them. I'll do that.
[55:46] - Good idea. - We can do that, you know, after this,
[55:50] but yes, needs-based decision-making. - Needs-based decision-making.
[55:58] Thank you. Yes, thank you, Homie.
[56:02] Great question and awesome. It looks like we walked away with a lot of to-dos list,
[56:08] at least for myself, of breaking down a lot of what I was learning to ask the questions
[56:15] 'cause today I was just more like observing it because I was like, I kinda get it, don't get it.
[56:21] And that's one of the things I think is awesome with the show and these videos
[56:27] is I at least know what to go look for instead of just not knowing what I don't know.
[56:34] - Once you use Docker, I'm telling you, you're gonna use it like every day.
[56:40] Like I use Docker every day. I also use Kubernetes every day,
[56:44] mainly 'cause I'm building training on it, but I do like have a cluster running
[56:47] on a Linux machine at home too. And it's just like, I'm always like, okay,
[56:51] I need to use Docker to run this task or whatever. In fact, to give you a practical application
[56:57] of something that I actually use at home, like in production at home, is I just have a little,
[57:03] do you know what a Raspberry Pi is? It's like, I don't have one handy right now,
[57:06] but they're just these little like micro single board computers.
[57:10] And I've got a bunch of them 'cause they're dirt cheap to buy,
[57:14] but you can run different applications like InfluxDB on them.
[57:17] And so I use Docker to run this InfluxDB web application. And if you want, I can actually show you
[57:24] what it looks like, but it's really cool. It basically just allows you to store metrics
[57:31] and graph metrics. Uh-oh.
[57:34] - Maybe, maybe. - Yeah, is it gonna load?
[57:39] - Here, I'll go back to us and then. - It's loading.
[57:42] - There we go. Cool.
[57:44] - Okay, there we go. So this is InfluxDB.
[57:48] Again, basically a single command to launch it just like we had with Neo4j
[57:54] or any other container based application. But what you can do is you can create these buckets
[58:00] where you can store metrics inside of. And so I've got this dashboard right over here
[58:06] that I've created that has like weather data. It's got performance data.
[58:14] So it's like pinging trevorsullivan.net to see how long it takes to load.
[58:18] So I can see how long it takes to perform DNS queries or how long it takes to access a website
[58:24] or what ping times I have to different devices on my network. And so this is just kind of a way to like gather data
[58:31] and then graph that data and put it into a meaningful format that you can consume personally.
[58:37] And InfluxDB is open source, it's free. You can run it yourself.
[58:41] And then there's this agent called Telegraph that I also run on the same machine as InfluxDB itself.
[58:47] And that Telegraph agent is what's actually gathering the metrics
[58:51] and then sending them to InfluxDB here. And then InfluxDB has what has this web interface
[58:57] that allows me to actually graph the metrics and kind of make sense of things.
[59:01] So I can add, you know, cells here. I can run queries against different bits of data.
[59:07] If I want SNMP data from network devices, I can grab that and build a graph around it
[59:13] and then add that to my dashboard here. Oh, here it is.
[59:20] So it's just really cool. It allows you to kind of graph data.
[59:24] - That's fun. - Yeah, and it's colorful and it just looks really nice.
[59:29] And it's just so, it's just, it's easy to use. Like I love software that's easy to use
[59:34] and InfluxDB is easy to use. - I dig it, I dig it.
[59:39] And homie coder says sick dashboard. (laughs)
[59:44] - Thank you. You can build your own very easily
[59:47] with Docker and InfluxDB and Telegraph. - So that was Docker, InfluxDB,
[59:56] and what was the other one? - Telegraph, T-L-E-G-R-A-F.
[60:02] So the company called InfluxData that makes InfluxDB, they also make that Telegraph agent,
[60:12] which is also open source software. And it's got all these different plugins.
[60:16] And I've actually got some training at CBT Nuggets that talks about like how to configure Telegraph
[60:20] to monitor network devices and basically all the stuff that we're kind of looking at here
[60:24] and understand how to gather data and then send it to a database like InfluxDB.
[60:33] But it also supports a lot of different output plugins. So InfluxDB is just one of the targets
[60:38] that's supported by Telegraph. But if you wanted to use a different database engine
[60:43] besides InfluxDB, you could use, there's a whole bunch of different database engines
[60:48] out there that you can store data in besides InfluxDB. There's like TIDB, there's timescale DB.
[60:55] Yeah, there's a whole bunch of different database engines out there that store metrics.
[61:03] - Interesting, interesting. So again, lots of homework to look into.
[61:07] I'm enjoying it. And thank you again for hanging out with us today, Trevor.
[61:12] I know we all appreciate it. And y'all, if you have questions, of course,
[61:17] hit us up on YouTube or go hit Trevor up on Twitter. And Rivet says, oh, yay.
[61:30] This was a great one. Rivet's a big burning question
[61:34] that they've been carrying around since they first heard of Docker got answered.
[61:38] So yay, awesome. And for everybody, make sure that you follow us on Twitch,
[61:45] have more guests like Trevor and possibly Trevor again, if we can convince them, we'll see.
[61:50] And thank you everyone, bye. - Thank you.
[61:53] [BLANK_AUDIO] 
