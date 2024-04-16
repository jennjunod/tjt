---
showLink: "https://www.youtube.com/watch?v=H6E5BJHdKFY"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "jenn-makes-tech-learning-postgresql-pt-4"
title: "Jenn Makes Tech: Learning PostgreSQL Pt 4"
publishDate: "2023-04-20"
coverImage: "https://i.ytimg.com/vi/H6E5BJHdKFY/maxresdefault.jpg"
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

[00:00] you you
[00:04] you you
[00:08] you you
[00:12] you you
[00:16] you you
[00:20] you you
[00:24] you you
[00:28] you you
[00:32] you you
[00:37] you you
[00:41] you you
[00:45] you you
[00:49] you you
[00:53] you you
[00:57] you you
[01:01] you you
[01:05] you you
[01:10] you you
[01:14] you you
[01:18] you you
[01:22] you you
[01:26] you you
[01:30] you you
[01:34] you you
[01:38] you you
[01:43] you you
[01:47] you you
[01:51] you you
[01:55] you you
[01:59] you you
[02:03] you you
[02:07] you you
[02:11] you you
[02:15] you you
[02:20] you you
[02:24] you you
[02:28] you you
[02:32] you you
[02:36] you you
[02:40] you you
[02:44] you you
[02:48] you you
[02:53] you you
[02:57] you you
[03:01] you you
[03:05] you you
[03:09] you you
[03:13] you you
[03:17] you you
[03:21] you you
[03:26] you you
[03:30] you you
[03:34] you you
[03:38] you you
[03:42] you you
[03:46] you you
[03:50] you you
[03:54] you you
[03:58] you you
[04:03] you you
[04:07] you you
[04:11] you you
[04:15] you you
[04:19] you you
[04:24] you you
[04:28] you okay that's fun haven't done that yet
[04:55] transitions are going to be a bit of work but that is okay hello hello beautiful humans welcome to another episode of teach gen tech or we're trying out a new name of gen makes tech thank you ramon
[05:10] i appreciate the idea for that one i am gonna hope that i actually have audio since this has happened before let's see if i hear myself uh oh i don't hear myself why don't i hear myself
[05:24] that's never good oh because i probably have the tab muted that's always fun uh a mute tab yay in a weird way it is great that i can hear myself that means you know if josh stops by
[05:42] the stream like half hour into it i'm at least probably gonna have sound that is improvement okay so oh my god itchy do do do do we are gonna do some postgres stuff today
[06:02] and i may or may not have looked into like any of it yet i was just like hey we're gonna get to the computer and then we're gonna figure it out that is that was the motto for today
[06:19] it's gonna be great sure give me a moment make sure i got we got the ipad going oh look yay
[06:33] i do also really need to add that to like my about area oh yeah that is something that i have yet to do is really fill out the like about if you see like some streamers have it
[06:50] like really well filled out and then other people are just like yeah whatever i am working on i will get there i will get there there's a lot of automation and things that i i want to do in life
[07:01] yet the energy and time does not always match it it's annoying but i feel like that's just part of the human condition that's just like everybody okay let me go i have notes that
[07:19] i created for last time so let me i will say y'all like last week was so fun because dan ended up reading into the stream
[07:33] and then also joined the stream yeah i didn't do anything after that like i'm supposed to i should could could have i don't want to say should i don't like the term should could have
[07:46] streamed again last week yet i didn't so here we are doing week four during week five and then i'm off for two weeks but i feel like we can we can tackle the rest of the to-do list today so i can
[07:59] start making my actual videos on how to do all this and now i just have to find what i did with all the documentation and once i do that and then i can start sharing my screen but i see a few of
[08:14] you are starting to join so how are you what are you up to doing anything fun today tonight kind of matters where you are in the world this morning wherever you are
[08:29] no i need postgres learning boy at one point i had i thought i had this mostly figured out
[08:42] not always and as you can tell i probably will have the sniffles today which is so annoying no matter how many allergy pills or anything
[08:52] i always have the sniffles let's see shared with me there we go no not that one damn it aha is this it this is it
[09:14] sweet and then we are going to do this yes okay
[09:24] do do do you do i don't know if y'all ever do this but i feel like it is worth sharing i was out walking
[09:49] the dog and thinking about how to set this up and just like finding what i'm working on today is part of it is like querying content and i'm like i said out loud oh that shouldn't be so hard
[10:02] to figure out and i'm like oh you you can tell i'm a streamer or i just awkwardly talk to myself one or the other but um yeah that happened that was cool i'm glad no one was around
[10:16] could have been embarrassing but i feel like my neighbors already know that but i do this stuff yeah i don't know
[10:32] yay sniffle sniffle sniffle come on i'm sick of these sniffles postgres postgres
[10:45] okay y'all let's do this and i will share my screen and if anyone's curious i really do need to get all my lighting uh and work on it and bring some more orange into my life because
[11:01] i promise i am not some weird shade of blue i'm gonna go with i'm going for something for it you know it's
[11:11] the new trend yeah let's go with that it's a new trend to be more blue and have blue skin that might be a 90s thing i don't know it's okay
[11:29] entire screen that one yay i'm glad you got it i always feel like so silly when i'm like uh did anyone get my reference okay so i worked very hard
[11:49] on cleaning up this docu doc document i almost said docu sign which if over on my ipad if i'm looking at it this is basically what we've gone through so far and thank you for the follow i
[12:05] appreciate it oh yes what was the last impromptu song do you ever remember them or is it just like a you never know what radio station you're going to be listening to
[12:22] this is what we did last week or last few weeks and i feel oh i need to put notes on here
[12:33] yes okay so i have before this like give you some background i have been in the tech world or tech adjacent almost my entire career i was tech sales i was tech support i worked in a call
[12:51] center i worked at go daddy i worked you know i tried video production for a hot minute i've been around data and tech what i didn't realize was how hard it would be to set up locally
[13:09] for postgres and i'm doing something a little new on a lot of my show there are people that come on and teach me about the tech well i decided that with postgres i'm just gonna wing it
[13:25] and we're just gonna see what i can figure out oh that happens i talk with my hands and hit buttons with my my pen uh and yeah so that's what happened first week one week two was
[13:39] a bit of a struggle but we got there uh luckily it was uh nor was there and then also uh week three was a lot of i don't know that didn't that didn't really work and then week four is what
[13:55] we're doing today so and oh was it the katie perry firework then because i was listening to the champion one
[14:09] oh what are you doing with postgres hey
[14:27] and if anybody wants amusement here is the playlist to hang out oh nice
[14:41] oh sweet i'm guessing that is live on github it's i think i'm part of that discord
[14:57] part of that discord i don't even know where discord is on my computer right now and there it is too many windows on top of each other
[15:15] oh yay well i don't know oh am i on the uh like streamers thing that's cool that's exciting i don't know is i i join a lot of discords okay let me say that i joined a discord because like
[15:36] somebody is super cool and i'm like i want to be a part of your discord that's awesome and then i like get lost of like oh there's so many people i don't know who to talk to i'm
[15:48] i'm really overwhelmed so i just end up sticking to my open source raid guilds with jacob oh yay hey that's cool well fancy thank you okay well i'm glad that i know that i was a
[16:05] part of that discord because i'm like that sounds awfully familiar or wonderfully familiar i'm not sure how you would say that but that is okay all right postgres you and i are going to be friends
[16:21] it's going to happen oh yes a lot of people i i talk a lot about mental health and neurodiversity as well
[16:36] especially in tech and a lot of people have asked me and they're like jen do you have a discord and i'm like no no no i'm not gonna it's not gonna happen i don't want to have my own discord i get
[16:51] lost enough having everybody else's discords but that being said since i hang out in open source rate guilt they mentioned that i might be able to have like my own like little channels
[17:02] i'm like that could be cool but i get to still hang out with people okay i need to actually do this
[17:15] and i don't know if anybody else goes through this where it's like you're you first go into a project and you're like i don't want to start this i don't want
[17:31] to start this there's like a struggle to start and then it's like oh okay cool like i'm a few minutes into it i'm good that is how i am at least every single time it's fine it's fine totally okay
[17:47] and we're gonna cheat and look at my notes and see what i did yes yes six days ago bananas
[18:14] oh i actually just started using docker for this project i started working goodness oh my gosh it's been 60 days oh that's so weird i started working at a data infrastructure company called ivan
[18:37] and part of my job is going to be to create the get started videos for this for postgres for redis and for my sequel i'm like i don't know any of them so i am learning
[18:52] them and docker was the first place i second place i tried learning them as the reason that it says local now and yes ramon you weren't here at the very beginning but i even said thanks ramon
[19:06] for the title idea so i think that's just what i'm going to do when i'm like learning doing something by myself jen makes tech learning blah blah blah but the rest of the time if it's a guest
[19:20] then it can be teach job pack that's what i'm going with pg admin ports and log in please keep my log in please keep my log in thank you oh
[19:37] we gotta go upgrade i don't want to think about this
[19:46] i feel like i should probably write think about this agreed agreed it is always pleasant when you don't have to sign in every time it kind of
[20:09] reminds me of my stream yesterday about apis when you don't have to do the handshake every single time not the same thing but loosely related ideas maintain what uh
[20:27] how do i need to update it we can do
[21:02] i don't know if i like clicked out of this way too much or okay that's that we're gonna go
[21:15] i'm looking over here and it says download maintainer docker container pg admin it's available at docker hub see instructions for docker hub
[21:35] yes i am reading these out loud so that way i hopefully don't skip words okay pg admin for
[21:53] aha full command ramon i blame you since you were one of my first guests it was a lot of like
[22:03] you were like you could yeah it helps to read the comments out loud although i will say now that i only streamed one area i don't read the comments out loud
[22:18] because i'm like yeah people should be able to see what others are saying because it's all in one area unless it's like super funny or important if you like i don't remember how to do
[22:32] this yes i do um we're gonna see if i can break some stuff no okay uh have i tried bionic reading thing
[22:50] um i've seen it heard of it haven't what's it sounds more interesting than me trying to unfigure figure this out so i'll allow the
[23:06] distraction the distraction good like i've seen things about it i haven't actually gone to try it yet or i just broke
[23:20] the website go back you don't want to load so we'll try something else how to geek oh um let's see
[23:37] it's not bad i um i will say i don't know like this is i a variation of it but yeah i i would say at least for this one as i was reading through it i still noticed
[24:08] that i skipped like this center complete the world and i skipped to bionic reading but it does make it a lot easier reading line by line or like across the line when i read something
[24:22] on this i can do a okay so when i like that bionic reading definitely did help me go like from here to here where
[24:38] normally i go from here to here to here to here kind of here and i still skip lines so reading out loud i at least have to like do my best not skip another one i don't know why it helps so
[24:55] much but it does it's just embarrassing when i don't know how to sound something out but that is part of learning live and streaming it's the fun part back here okay let's do how to update
[25:22] the pgadmin for on docker container steps can you hold the latest docker image stop the running container remove existing container
[25:50] oh you have to redeploy it to update it
[26:07] there's a video maybe i'll watch it really quick
[26:19] see if it helps playback speed yeah oh no it's just installing i want to update
[26:47] it says the same thing what do you like okay why do we have to update it oh you're good i mean that's part of the fun of streaming i am not a happy camper about having
[27:01] to figure out how to update that hey that is part of the process yay oh it helps if i actually share
[27:28] probably going to be easier this way this time yes yes that is why i take notes yes they're handwritten notes but that is a big reason i
[27:41] take notes because like oh how did i do that i don't remember you know what i'm just
[27:58] oh that is a good call that is a good call i'm also thinking about so part of like the how-to videos i'm going to be doing for work are using the trial so i'm almost wondering
[28:19] because it wouldn't be using a docker image i'm like would that be easier i wonder i don't know yeah i'm gonna go try it i'll just sidetrack myself and see if i can
[28:32] do the rest of it over there goodbye docker image i do not like you goodbye and let's see
[28:46] do that over here get started for free
[29:02] sign up with google i have too many email addresses
[29:11] oh um well something about on here is really quick as like a side note if i do let's see if i hand write your name this is it's supposed to happen j o d a b
[29:41] a if i go to like the main area i'm supposed to be supposed to be well we'll find out if this actually happens let me make this bigger again so i wrote your name and now i'm gonna go
[29:56] search search and it shows up uh one match and it highlights it isn't that cool yeah yeah it's so cool i'm gonna erase your name though because that's what's gonna be weird i'm gonna be like
[30:28] what about this person or name i don't remember when i look at it in like three months okay yay oh oh i wonder if i'm not going to be able to create the free service let's see
[30:48] aws i am in north america and aha it's down there we can be central that's fine we're gonna do name this thing what do we name this learning
[31:12] postgres we will do that create free service yay oh goodness gracious um oh there's a lot okay
[31:30] secure connection whoa
[31:39] well hello hello rivet thanks for joining i was and i'll go back through this really quick just so that way you can see um do you i can zoom this in a bit so week one i well i've been learning pg
[32:05] uh wait postgres it's uh oh yeah anything that i do on my stream i'm gonna redo for other things like luckily if i do it on stream it's not gonna be anything public thank goodness um i'm setting
[32:20] up a postgres and i'm learning it without ever doing anything so the first step was week one trying to set up locally that was absolute [ __ ] it was painful it was a very painful time in my life
[32:34] then week two let's try docker okay let's do it we will try docker week three was secure your connection manage users and permissions and create schemas
[32:50] which i got stuck on step number one of week three it was kind of yeah and i have been taking notes on what i've been doing to get to where i'm at yet questions questions look at this
[33:08] does secure connection mean ssl because i couldn't like find what it was looking for and i logged into pg admin today through my doctor instance and uh it's like yo bro you need upgrade
[33:25] and everything that it was saying was all the googles were basically saying hey to upgrade your instance and for pg admin you have to delete the old one and then reinstall it and i was like
[33:40] oh god i do not want to do that again so why not go set it up on ivan since we have the free tier now why not i need to learn postgres overall might as well make it easier on myself and see
[33:53] like compare it just in my own mind and connection and this this step that i got very stuck on for the docker one is like literally just really easy right here what what how
[34:17] i did ask uh like between my streams something that's really cool about the team i work with is they all know that i'm a noob at this and so i'll ask some questions especially like hey is
[34:30] this like a pg admin type thing or is this like because i'm doing it on docker or is it because like how is it on ivan and from what i understand is that ivan would automatically secure the
[34:47] connection i am curious like how railway does it because i did um anthony campolo did show me that it's even railway is pretty easy to set up too so let's stick this skip this step oh hey
[35:05] we can migrate or sample data uh let's skip this step oh there's extensions and things
[35:17] i don't know what those mean yet so we will uh skip that and yes i may be excited about pg admin because of the elephants
[35:33] don't judge thanks okay so oh you can just like upgrade the version there
[35:46] uh is it thank you thank you and do i say i i should ask do you say it joe dabba jaw dabba
[36:04] i'm really bad at these uh uh ssl secure socket layer is the encryption protocol and we now have tls which is a bit better but everybody's calls it ssl still even though it's
[36:18] not always actually ssl things get confusing really fast on the security front um i call it job security yeah yeah i dig it i dig it
[36:29] yes that is the happiest news well joe dabba it's gonna go with what i'm going with now i completely agree on the ssl stuff
[36:46] it was very confusing looking how to secure it and even looking to um look this up in like pg admin i think this is gonna boot me out because i killed it on docker yeah you're not even gonna
[37:01] work that's fine leave site yes please okay yes close out of all of this close so many things close close yay
[37:19] quick net oh psql cli pg admin what oh yeah for sure thank you for the suggestion
[37:49] look ramon this is like the first time i'm actually like fully going into like checking out the item stuff so that's why i'm like whoa it does this that's really cool
[38:06] like it was really difficult googling at the last like three streams and just being able to ssl mode require the ssl is just on what and we can do a quick connect
[38:20] oh i was just saying that it like it just does the things it does things without me realizing that it does things like easily
[38:37] uh sorry i by the way i have ads turned off i don't know why it's still well this one
[39:01] oh maybe i need to delete this one delete service i'm deleting my old services that i had on here when i was applying because i don't need these
[39:26] mysql ones we'll get to mysql someday we're not there today i need
[39:35] so you should go away filling information oh that's fine you don't need a payment method okay so if we're here
[39:51] oh there's queries and users and databases we can create a new database users are so much easier
[40:04] what is this okay so
[40:36] i feel like i should not be this excited about it that it's just like seems very simple okay so i'm going to quick connect i'm choosing pgadmin connect ivan to be
[40:50] a post sql database with pgadmin you can easily import a new database connections to pgadmin with a json file open pgadmin and click tools
[41:04] remote you might know this one does that mean i need to have pgadmin on my computer or wait i think i do do i i do maybe
[41:21] what just happened oh it took a minute that is what happened waiting for pgadmin 4 to start
[41:34] uh let's exit that let's exit that oh you guys can't see it i can't see it
[41:47] uh let's exit that let's exit that oh you guys can't see my master password that's not for you that's for me
[42:12] okay okay uh no
[42:27] please don't tell me you're gonna make me install again can't you just update yourself bro like come on
[42:37] um okay click here for more information and i'm not
[42:47] why doesn't it just update by itself why do i have to uninstall and reinstall will it replace itself
[43:14] yes yes i call a lot of things bro i i don't know if that's a good thing or not see look like this is odd just because we've talked about having to move things to applications
[43:32] this one doesn't even have you move it to applications yes i want to open it
[43:42] please load this is going to make me have different instances can you replace my current one
[43:55] replace the current one replace it go
[44:02] fine fine there we go leave this is the really fun part about streaming when you have to reset everything and reset stuff up yay
[44:24] yay ramon when we were talking about querying stuff earlier i
[44:40] am excited not excited i will tell you that i'm excited technical difficulties banner probably
[44:53] or gen clicky clicky too much what's oh i don't need stack builder actually thanks but no thanks i don't need you at the
[45:10] moment yes i want to exit you okay let's try this again pg admin 4 hopefully you are the proper one well you know uh i've tried it a few times that's about it so we'll learn together it'll be fun
[45:34] as soon as oh why are you opening on this other window that's rude i do like the colors it's pretty
[45:46] and then look at the elephants yay uh you know please start please be magic yay i literally just did this like
[46:14] okay apparently there we go and there we go okay so we have pg admin that is great we are getting somewhere swipe up unlock tablet please thank you so what i'm going to do really quick let's move
[46:41] this out of the way let's there we go and you're just going to be an awkward size somewhere i'll just zoom you in really really a lot yeah that's that's some good english really a lot okay and
[47:01] so if i'm taking a look at my notes i'm just crossing out what i've already done because i did follow my instructions on like steps i've taken for setting it up on docker
[47:19] like i was following all of this and it wasn't be my friend it wanted to uninstall and reinstall stuff so we had to set up an ivan so step number one cross this out because we decided to not do
[47:39] that and step number two is you know i've been uh create i've been count that was pretty easy and i need to write down my oh too zoomed in now
[48:06] unzoom in thank you thank you and then we went through all those steps i basically just hit next next next and now we are on get started oh wrong one
[48:30] oh quick connect okay quick connect
[48:39] and it says open pg admin
[48:54] and import export servers okay cool i will say that considering this is my steps from last time it seems a lot easier to do in
[49:11] ivan just because like i didn't have to set up docker i did have to set up the same account so we'll say give me a line thank you
[49:27] since i'm gonna write a little bit i will do this it was account
[49:41] setup we're the same but i didn't have to install docker
[49:52] like i had to install docker but not install ivan and then install postgres sql on docker nope didn't have to do
[50:01] yay and set up a client okay that is where we're on that's gonna be fun let's go try it give me this can you zoom in oh you can yay
[50:26] okay so quick connect create a json file click tools that means i have to find tools processes sql
[50:51] oh up there that does make sense import export import pg connect
[51:11] json yeah we're gonna remove everything since this is our first one in here let's hit next
[51:26] oh oh because i can't see everything that would help oh okay
[51:43] um okay that's fine
[52:06] so this doesn't need to be there anymore but nope come back oh there you are desktop
[52:33] so and we are going to do
[52:48] new folder learn postgres and
[53:03] oh i guess that's not what i actually wanted i wanted hyper yes oh my goodness all the updates at least this one's faster unless
[53:26] learn postgres sweet cd learn postgres oh that yay
[53:37] we need a new file it needs to see what pg connect dot json
[53:51] pg connect dot json yay paste sweet save
[54:07] you can edit the variable name and group name
[54:17] name pg1
[54:29] good enough for me all right going back to pg admin we then wanted to go to tools import go find this thing
[54:44] nope desktop code learning postgres this dot json yay and yes delete everything that's we're not using select group servers yay summary finish
[55:13] please select connect the selected server to the view in the dashboard really good thing that i'm not going to be using this for everything because
[55:40] yeah i'm showing passwords on on stream you're not supposed to do that y'all just as a heads up i on the other hand am not worrying about it because i am learning all of this live so
[55:51] when i go to make things it won't oh well y'all this is even i feel like this is even easier than
[56:08] when i installed it through docker like even the pg admin looks easier i don't know we could be making things up i will go verify okay so
[56:20] do i have a favorite animal yes it's one of the reasons why i love postgres it's the animal of postgres now now you gotta knowledge check yourself do you know what that
[56:40] animal is i don't even know what that is is that a type of elephant
[57:09] i hope this isn't going to be a bad google oh my god those are cute those are cute but no you know what i really want is a
[57:29] uh what are they giant rodent yes i copy bara
[57:41] look at these things yes yes i want one look at them they are cute they are cuddly they are cute and cuddly and they're big big i want one
[58:00] i went down a google rabbit hole one day and found out about all this stuff and they're really cute and they can like be really mean and vicious but um
[58:13] they're normally very cute and very friendly yes yes so everyone should get one of these okay back to notes we imported it to pg admin
[58:34] i don't think there's anything else i need to do to connect them no we are caught up yo i got caught up switching over to ivan what took me like
[58:52] like 12 hours to do previously we did in an hour to get caught up to this point yes what up allison how's it going thank you for joining us we are setting up postgres and gonna try to do some
[59:06] things currently this is what we're looking at uh in this handy dandy corner is load some data you know what okay just eh e there maybe that'll work if i just keep it in the corner i don't know
[59:27] so let's go try to find right i was like i need to find sample data sample data for postgres sequel
[59:47] oh uh postgres is one of those words you hear and you get bored i will say okay it's i've been working on learning it from scratch meaning that like i didn't do any googles i haven't
[60:13] had a guest on my show about it it is something that installing locally was very difficult installing on docker was less difficult and what i'm using right now has probably been the easiest
[60:32] i also like i i guess i just don't want it to seem like it's just a promotion of where i work because it's honestly i just did it in an hour what i was trying to do the last three weeks
[60:48] and it's a bit eye-opening when it can be something that easy and it's free yet i would check out my if you want to see like what i did to set it up in the different versions i will go
[61:02] look at the youtube's youtube youtube this way oh i don't want to verify it's me can you just go to my youtube bro
[61:11] i don't know why today is very password authentication heavy it's not it's not fun it is not fun you guys can see my stats it's okay it is a growing channel oh hey
[61:36] that was yesterday's stream it already has 14 views and two likes that is exciting uh play this setting a postgres this is it shareable link so each week it goes through like what i've done
[61:55] so far so if you're like you want to check it out totally do i can also show you my notes here is week one i try to set up local and that is why it says no i would not suggest it to anybody
[62:17] and then week two i set up docker that to me and why i'm like leaning towards the place that i am employed is setting up docker i had to learn docker which i had never used docker before
[62:35] that's why a buddy of mine actually came on stream after that one and was like jen you should probably learn a little bit about docker i did it was very helpful and then week three was securing the
[62:47] connection and i spent so much time looking up uh like the ssl for it or the tls um as was mentioned earlier and then also managing users and permissions and creating the schemas
[63:02] it was all just kind of confusing so and it was still with pg admin yet it looked a bit different than this but i don't know if that's because of what i installed
[63:15] on docker or because this just had an update but on my place of employment it also just said yo dude you want to like add a user go to users
[63:30] yeah you you want to you know do some security and get started let's do it let's secure your connection and that's kind of why i was like in shock i was like wait this is like telling me how
[63:45] to do stuff very easily skip this step i can even add data from here we're not going to do that but we could we might i don't know i'm not to that point yet i haven't found the data i'm going to
[63:57] upload and i'm trying it because i need to learn all this and it's where i work i as a developer advocate there i will be creating how-to videos so i'm i'm stoked oh thank you
[64:18] so y'all i don't know what i just clicked i just clicked something and it like took me away
[64:39] i don't i don't know but thank you allison um it's i was going to reply to you yeah apparently i got excited and click stuff that is that does that does tend to happen yes uh ivan has been so
[64:53] dope they are very supportive about me learning live and knowing that i need to learn a lot like continue learning to be the best developer advocate i can be and then also one of the
[65:07] other reasons i'm learning postgres is so i can put all of my past videos and pat and past podcast episodes on my website so just like a little side note y'all you can kind of see what i'm working on
[65:22] okay uh so that's me if i'm wearing glasses and my leather jacket and this is also me a little bit more about me but i have these three things going on oh you guys can't see it i hate when i do that
[65:41] something breaks and they're like and people are like dude you're not you're not sharing your screen yeah yeah i that would help i wonder if they ever have like the awkward streamer awards
[65:53] because if they did i still think i would win anyway hey there you go that's my photo that's about me and these are the three projects i have you can now see what i'm looking at
[66:06] which is exciting i am working ramon i feel like we would have to tie from most awkward we could tie it is something is one of the the the fun things about streaming and doing live streaming is uh
[66:27] you'll learn to be okay with being awkward and what i want to do with all three of these which we'll do here
[66:37] mirror board zoom out zoom out is zoom in on the website i want to be able to make it easier to stay and be able to put all the podcast stuff
[66:59] here and live stream stuff and uh this is process i'm going so far and you've been using uh postgres the last couple days with directus a cms built from databases and you're building it for a
[67:17] personal website that you're going to bring up cool if you're open to learning other ones i mean this is just me also learning about the company i work for too because i'm doing uh
[67:31] the free tier of ivan just to do it and compare to you and i've i haven't used directus yet it was super easy to connect and to get over to pg admin so on that note i'm like literally just
[67:49] wanting to curious how it compares than anything okay that why do you keep locking on me this is this is definitely it
[68:01] also oh i need to i should tag him and what are you building on your website allison
[68:14] oh okay okay that makes sense ish i will say i just did a stream about hosting because i come from a shared hosting background so now going into like learning then learning javascript
[68:45] and then learning like about for sell and netlify and things i'm like wait a second this is all a lot different than shared hosting
[68:54] it's a uh well it does have some of that but it's more of the data infrastructure itself like the managing the databases and being able to um so that way you don't have to go through
[69:12] and set it up and manage with like aws it does it for you so you get to have this all in one nice little thing box though i will say
[69:24] you ask me in a couple months that might be different and have a deeper better explanation and what is this human's name we need to shout out this human because
[69:41] they have really good stream music and i don't remember i'm jealous oh yay i built i'm building my site with astro as well
[70:03] actually i have that as part of over here because it's been like people have asked like what i've been building with so i've been trying to uh like showcase it and see what i'm
[70:20] doing so ah yeah yeah it took a while i got really stuck on things weren't adjusting properly for me for this so when i went into like mobile it wasn't looking great but a lot of it had to do with
[70:41] some of the customizations i did but then also um the the the person that made the theme because i'm using this brutal theme is going to come on the stream sometime i'm very excited it's going
[70:54] to be great but oh they're streaming right now we're still going to get because they always have really good music okay let me know how you build out your architecture i'd love to have a
[71:17] conversation about that because since i started learning how to do all of this it's been a lot more of the front end and i will say after starting at ivan and i'm just so curious about
[71:31] the architecture side i'm like dude data architecture is just like so cool yet i it's harder to see instant like you know gratification like you can with front end at least in my
[71:48] experience let's do these let's do these okay so sam griffin has the best music music
[72:04] okay that's not how you spell music yay um so i would just yeah
[72:21] he has the best music music there we go i can i can put things i can write
[72:38] uh i'm thinking about it because i'm like i don't have any music going i really want some music
[72:45] but i don't want to figure out the royalty-free stuff at the moment focus jen focus we can do this okay we need to go back to sample data
[72:59] sample data yes yes let's download the post-sequel sample database
[73:14] oh i'm going through options really quick oh look sample databases wow this website is hard to read
[73:29] okay uh many database systems provide a sample databases with the product
[73:38] a good entry to popular discussions blah blah nice yay i love meeting you cool dope people
[73:51] dope people it's what it's about databases databases add a database name name maru
[74:08] that is gonna be your name i made the database and databases what's wrong with this one oh
[74:29] okay that's cool it didn't import anything just created the name okay let's yay
[74:41] oh dude that is so dope yes do you have the twitters go hit me up on twitter because that's i can show you my twitter it is on my i think it's on my website i don't know
[74:56] yes yes it is go ahead at my twitters i should probably tell people i'm live now that would let's do that right now and we're live and
[75:13] have been for about an hour whoops where's the funny emoji
[75:31] i should say i'm live i mean i guess i have multiple person i i'm in gemini so sometimes people say gemini's have multiple personalities but i always go with the default if we what
[75:49] notifications do we have hey i got your follow let's follow you yay okay focus if i want to
[76:04] import it looks like it was just the get started add data this one does have load sample data
[76:16] we're gonna see what it decides to do uh oh database imported okay
[76:30] is there a way to reset you refresh
[76:53] application user background worker launcher oh what is that doesn't look great well let's can't oh
[77:11] pg1 icon on the left i can ah refresh good call i don't know why if it's just like because of
[77:28] it being like you have to right click it that it just doesn't make sense to me okay why are the rest of these like not okay that one connected i deleted namaroo
[77:40] uh i don't even exist i just have defaults so we're just gonna delete and drop this one oh okay
[77:56] oh namaroo is back whatever dude let's go look at paglia gilia oh yeah that does make sense that does totally make sense
[78:18] but hey we have we have things here and do huh
[78:44] interesting those questions okay well query tool that is the next point is to query and
[78:58] interesting i've never actually written a query in fact ramon and i were talking about this today and i was like you know what i'm gonna figure that out today
[79:15] let's this new query tool let's learn the query oh yeah that's actually a big thing that ramon was talking about if you if nobody if nobody
[79:37] if y'all haven't followed ramon yet you should let's see if i can do a shout out shout out shout shout out and then at ramon oh hola soy milk
[79:52] hola soy milk yay y'all should follow hola soy milk he also streams a lot of content and is one of the main people reasons that i do stream and also it is
[80:10] a lot to do with learning exit exit exit exit all the things okay
[80:28] oh okay standards so learning the sql query language can expand you know others as well kind of like each language has its for loop oh yeah yeah and rivet you're a
[80:43] big fan of the w3 school's sql tutorial reference oh interesting i'm curious do you guys say sql or sql because like i think i use both without realizing it
[81:00] oh let's go look at this interesting i i honestly feel like i say both but i don't i don't know why it's kind of weird
[81:25] oh look exercise insert the missing statement from the columns huh
[81:36] this is cool so
[81:53] i say jason as well instead of jason hello hello deidre wow words deidre how can i not say i'm sorry i'm messing up your name completely right now but welcome welcome
[82:17] uh we are learning about postgres well i'm learning about postgres they kind of know more about postgres than i do at the moment but i'm gonna get there i will get there
[82:33] wonder top sql queries of sql queries
[82:48] most important sql queries in 2022 let's look it up yeah it would help if i spelled queries right thanks for auto what how did i do that
[83:00] i don't know how did i click this whoa um well apparently i'm learning stuff about google as well because i never knew that you
[83:13] could click this this is cool do i have a job yes yes i do have a job i work at ivan which is a data infrastructure company
[83:24] retrieving tables oh cool i think that's also going to be a part of it of like do
[83:43] like what commands are out there is something that i think is also very new of being able to do it from here
[83:53] i don't know so
[84:06] select query oh that's cool
[84:26] thank you both of you select from table name and see what i get okay okay yeah
[84:43] this is fun yes i will say this is so weird though like having to
[85:03] stumble through it a bit more instead of being able to like have a guest on teaching me through it but it is really fun of being able to you know learn it in a bit of a slower basis
[85:19] i this is actually something i know i'm i'm oddly pausing of
[85:32] oh there we go i didn't know what tables i had i was like i know my schema i don't know what tables i have but we have actor
[85:52] save run play execute no no whoa whoa is there an undo no okay we'll just make it fit back in there
[86:07] that was a little can you go back in there go back route oh okay there we go that'll work yes yes i will say being able to go through something that i have found is i don't know
[86:23] if it's something about just the way people have learned or like time frames that they learned like when they went to school or where they went to school
[86:38] rivet yes yes let's do it um that's awesome it's it's definitely something like i i purposely wanted to stumble through this with
[86:57] it's it's definitely something like i i purposely wanted to stumble through this with postgres to learn it so that way i really understood some of these spots that are harder to
[87:14] learn with by the time i got to ivan because when i was interviewing with ivan i did set up a trial before they had the free tier and i went and i set it up with prisma we had somebody on the show
[87:30] of uh from prisma and it was really cool yet i was like i i don't i don't know what we just did like i get it but i don't get it and i think i also didn't understand how difficult it was
[87:48] not realizing that without that knowledge because it was so easy when i used ivan before i started going down and looking at databases yet data infrastructure is so fascinating
[88:01] prisma streams stream okay there we go anybody that wants to look at that that would be dope and while you're there you know feel free to
[88:20] give me a follow because or subscribe youtube is subscribe because you can't actually like do a ton with youtube until you had uh so you have a thousand subs it's crazy rivet uh used to joke
[88:38] that the easiest way to get two devs to fight is to have them design a database schema together interesting and i think that's also one of the parts here let me go back to the ipad is
[88:53] go over there is last week or i guess two weeks ago now when i was looking into secure your connection that or we already talked about that that started making a lot more sense
[89:08] manage your users and permissions cool that made a lot of sense but then it was like create schemas and tables and i was like so what's the difference that is something that i still need
[89:21] to look into and do i don't know i don't think it'll work until won't have time till after i'm get back the next two weeks i'm gonna be gone it's gonna be crazy but i will pin that to my
[89:41] to somewhere saying that jen's out of town because i think actually actually uh what up how would i say your name oscryptor are you an australian cryptocurrency person
[90:03] that is what i got from your name tables are informed by the schema the schema defines what tables you have and what's in them okay that being said something that was really great feedback that
[90:18] i got on twitter which is so fun when you get like feedback they're like yeah you gotta talk about this is to do other crypt robber in austin texas all right all right that that is also a way that
[90:41] that could i could see that yeah but that i feel like a crypt robber would be more in like louisiana yes yes we do come join us on streams and then we will give you a new backstory it will be fun
[91:04] um so let me i know miro miro's scrolling way too fast when i was talking about on my website that i wanted these to be to like teach gen tech to have its own pages that would have the youtube
[91:24] embed video description guest contact associated links and then the transcripts where like the podcast side is going to be a bit more complicated it does need to have the youtube embed but
[91:36] the podcast link spotify link episode description guest contact associated links and then the stream so does that mean i would have two different schemas instead of two different tables
[91:52] because they have different content oh okay what did you think about our backstories for you uh as an australian security stuff cyber security
[92:09] as a instead of being a crypt robber from austin texas i still like that one though i'm wondering can we oh you could say that you are a crypt robber and you're stealing api keys
[92:29] just just saying like i'm trying to think of some security stuff stealing api keys from crypts that's security kind of uh would probably be a schema with
[92:42] multiple table tables but there are other uh dbas that will fight on that you've been coding for over 20 years as a freelance developer nice nice yes database
[92:58] administrator i did get that one um but i think a database administrator i always think of like at some point i should ask people this what is the difference between a database administrator
[93:12] and a sysadmin systems admin i don't actually know if there is a thing like what a system admin person does but uh oscrypter that is what type of development
[93:31] have you been doing was and is there something that originally got you into it or oh as like a total side note y'all ben gamble who has been on the show a few times about the
[93:47] the basics of data like y'all we are talking about like going from the cache to the cpu to you know to an ssr all hardware stuff and this is exciting
[94:02] he's gonna give me a raspberry pi to set up and i'm gonna see what i can do and i'm gonna stream it i am excited not excited
[94:15] okay okay this makes sense and thank you what about like i love getting into databases because this is like i don't know why i find it so fascinating
[94:38] but also feel very very silly uh of like what do you manage on a database that is so large is it doing these queries and if a query breaks or um oh i like uh
[94:57] oh allison that is a great call out thank you that is good to know and uh oscrypter i dig it
[95:08] okay okay interesting interesting so many things to learn and i will say uh
[95:22] right like that made sense like what you just said allison it makes sense to me like hey this is what goes into a database it's when we're going from let's say like actually
[95:43] going in to learn the queries and why you would query them i think is one of the harder things for me to conceptualize and then how in how am i gonna set that up to show up properly
[96:02] in my website because in the previous website i made i had multiple json files and there wasn't like one source of truth so that's why i'm like huh well interesting
[96:19] oh oh that's cool rivet interesting yes this might help let's go find my github let's go find github
[96:39] github it's this website but look this is my old astro website load load please load hey it loaded so this is when i was looking for a job i got a job so i don't need it
[97:00] to say hire me anymore and i didn't like that uh it was only one website so but if i go to my perf well okay if i go into the stream schedule it was where i had like a json file for all of these
[97:20] and then i would have a different json file for each of these components for code writing and speaking um db admin tend to monitor databases creating users ah okay okay that is good to know
[97:42] um let me i don't think i have it on my computer why am i being so blind do i not have hyper open anymore
[98:04] well i do okay i don't want to go log into all of it we'll just do this but i think it's the other website
[98:22] we can go delete that one that's fine go delete this one
[98:32] move to trash okay uh
[98:42] uh interesting no this is uh you both are everyone is bringing up really great points and i this
[99:02] is a big reason i do stream them is because it's helpful to learn and also it's like hey if some point down the road somebody is asking me these questions what will make it easier for
[99:17] others to learn about it where did i get stuck what is something that i can maybe help somebody else get through so i need to see the website
[99:29] okay i am bringing this up because this is like conceptually where i'm struggling of this is the astro website my first astro website that i built
[99:52] and under data i actually had to make they each had a json file that had an index file
[100:03] and that's why i was like so if i had a database i could tell this component to just load those things from the database
[100:17] instead of having to i think that's where i'm stuck it's like okay cool i can query the database then how do i attach it to the front end
[100:30] that is where i'm stuck yes and i believe that is what i'll be using i can close this too now yay
[100:45] uh prisma for i don't know if y'all have used or heard of prisma yeah go so
[100:55] yes yes um so i've done something in prisma and it was really easy to take a look at their content and this is and i think allison this is gonna take a place of direct us because
[101:19] prisma will connect the front to the back with the database that i created with ivan i also it sounds i don't know if this makes sense but like i want to test out ivan as well yes i'm
[101:37] learning it cool i work for them yes all of that i want to have my site set up on that so if i have errors that i can either work on getting them fixed or be like no bro like this is going to
[101:49] be a better option for you instead it's i like it so far but i also haven't stress tested it i guess you could say it's the word i'm looking for i want to stress test what i where i work
[102:05] yeah but i will be using this eventually eventually okay we can close this now that was exciting okay so that connected the database that was fun uh go back go back go back what am
[102:26] i doing so we queried it and what was after my that step oh my goodness it keeps logging i don't even know what that means well like i know what data types are
[102:43] oh that's cool do do oh that's cool
[103:04] do do do do do do do do let's paste this file
[103:33] copy file you have to copy it before you paste it oh wait wait paste data
[103:45] oh whoa that is really helpful allison thank you and see if you can find a table that's likely to have numbers
[104:03] and or dates and i can help with the data typing piece oh okay thank you interesting
[104:16] oh so would that mean that this top part would be part of the schema
[104:31] because it's telling me what part of how i would want my table set up or this would just be part of the table i mean i know it says my table create table but
[104:43] i'll look into that let me first look at find a table with these things okay uh i'm going to
[104:59] put this in here go in there thank you
[105:07] let's tweet about it pretty dope to use
[105:24] while figuring out json oh they already have json i'll delete it json to pestress ql and we can give the sql
[105:49] to json thanks at allison i don't know actually know what your name is on there oh my god
[106:03] something just got in my eye as i'm like oh i just saw it bam bam tweet it it happened um that command that creates part of the schema defines the schema creates the table
[106:24] oh i'm gonna say yes okay and oh my goodness eyeball please function what is that it has cool p on it
[106:43] properties but that only tells me the property of one thing i have to query it to see it all
[106:59] and i don't know oh wait okay rolls triggers film
[107:08] sniffles yes
[107:15] thank you thank you allison it was dope to have you hang out and i look forward to seeing you back and connecting
[107:29] thing okay is there a way yes i'm annoyingly clicking through these just because i
[107:55] don't exactly know what each of them do don't save this that's fine we don't need to save that query um there's constraints you can have constraints interesting okay let's see
[108:20] oh there's types of something
[108:47] okay and a query tool oh yay although i feel like your name makes people sad do
[109:00] people get sad that there's no free wi-fi for them and then one oh okay
[109:14] find no okay we don't need that how to
[109:34] find guys the select statement and for information schema are used column types oh
[110:02] interesting interesting uh now do a select from one of those tables that in that text field yeah would it just be like data type
[110:15] to tell me the data types it has okay
[110:32] i don't know let's find out what happens you don't like me
[110:49] uh start with my select so
[111:17] come on um
[111:55] okay so when doing it this way it shows that the data types are like integer text text timestamps are these the data types oh okay so address it's got address
[112:20] okay integer text text text small and small int text text timestamp oh see that pk
[112:38] um not at the moment i am very there is a lot going on on the screen oh yes pk yes
[112:51] oh hydro oh you can add stuff from here oh that's cool save results there's a graph visualizer primary key okay
[113:13] okay so it's like what it associates with because if i remember right postgres is it goes by the column so is it saying whatever the primary key is
[113:27] is what it will associate with for the entire column to like be its main id so i think that'll yay okay cool yay that's great i actually uh yesterday which revit you should
[113:49] definitely i i know my stream schedule has been [ __ ] i'm sorry and thank you for the call out it is such a good call out um yesterday's stream with ian we actually talked about the ids based on
[114:04] the um here i'll actually show you because it helped me click with this so let's go out and we're gonna go here apis oh my god it's very zoomed in but
[114:25] but we were talking about how the resource of like on this one is just to show a domain name just because a lot of my knowledge comes from shared hosting so it was a way of associating it
[114:44] is that is like the id but then as we're going into like looking into http verse one and version two is you can um we talked a lot about like with the ids of post put and patch and yes y'all i
[115:04] definitely said lipstick is like a patch changing lipstick is a patch changing your entire outfit but still calling it the same outfit is a put and creating the outfit
[115:17] is a post and that is how i figured it out but that reminds me of the databases because you with the put and the patch you can't change your id
[115:30] i don't know i don't know if that actually goes associates but in my head it did there are others that will say fk that marked how things relate to another foreign key okay let's
[115:45] see if any of these have foreign keys i don't know if they will nope time stamped is it
[116:02] interesting maybe payment um usually when you see a table that is name of two tables next to each other oh
[116:24] oh that's cool okay uh actor run okay scratch pad i don't want you here thank you
[116:36] uh let's do film category we feel i can type i can type we got this gen type category
[117:01] interesting it's like pulling the information but not like
[117:13] combining them because it is saying the category id and the film id oh okay okay well that's fun i feel like this did
[117:31] did definitely answer the questions i had to be able to get started today um or finish up today's uh go oh and monitor pg metrics and logs well that one was actually pretty easy
[117:56] let's go up here go to dashboards and i feel like we're monitoring them although we can also
[118:10] skip this finish because we can go to the logs here which learning postgres
[118:30] um shows me the user the database it was disconnected reconnected does it show that i actually like what i looked up i'm not going to go into like a ton of detail trying to figure
[118:47] out the logs but i at least know where to look at it in here and then the metrics which just look like very pretty graphs at the moment
[119:01] these are all things that i can go into later on and dive into because this is one thing that i have learned to love about tech is there is always something new to learn
[119:20] oh god data norm data normalization database normalization i'm gonna just google what it is database normalization
[119:35] organizing data in the database so is this like taking an already existing database that's like a hot mess and it's like
[119:47] hey here's the mess go fix it is that what data based normalization is fixing other people's messes that's what it sounds like
[119:58] yeah okay ideally you want to do it when you design the database up front but sometimes
[120:17] you have to do it after the fact okay i'm i would think that i would be creating my own database for like the show and stuff
[120:34] um so i guess i will learn how to uh you know create schemas yeah that that doesn't sound great that sounds very scary
[120:50] yet you know a year ago i never thought i would be excited about databases restructure the tables to optimize the queries and possibly reduce data duplication
[121:07] oh that is a yes rivet um at the moment it has become a very informal process of ways to sign up yet hit me up so i will i'm done sharing my screen because we are done for now
[121:25] i am checked out i say that as uh you know i've realized that about two hours is my like brain limit i'm like i've learned a lot in the last two hours yet i am feeling i am feeling optimistic
[121:42] because it's something that is making a lot more sense um chris rivet if i don't get back to you by tomorrow feel free to bug me for like the second week of may um i say that because as i was
[122:02] saying on linkedin is i am working on creating a better workflow i can show you guys this really quick because we were already looking at it share the screen so yes this is my lovely website goals
[122:18] and the tech i'm doing to learn all of it but before that there is this giant giant thing of how i was setting up stuff for the podcast and i want to do it for teach gen tech as well of
[122:38] i zoom in you know have a submission form that will auto schedule this stuff so that way i'm like okay cool i don't need to worry about all of this and i just started using hub spot again
[122:55] or for the first time so my hope is that i can set this up that i can be like hey chris give me this information and see if this works and if it doesn't well we'll just choose a date anyway
[123:09] and thank you for the follow oscrypter i i feel like i will forever remember your your name because the backstory that was created for you of
[123:24] australian cryptocurrency or you know austin crip breaker when in reality cyber security from australia that all makes sense and yes so automations we're gonna figure it out i will say
[123:49] ding ding we are getting there though because can we just like log in go to my account bro you're welcome is i was able to like the progress is getting there on all this behind the scenes
[124:12] stuff because on like yesterday's stream i was able to upload my notes from yesterday that i referenced to earlier and i uploaded this on hub spot so it could be its own graphic that
[124:30] people can look at and like you can zoom in and scroll around long long term like long long term is to get something to read my handwriting and just auto transcribe it for people that can make
[124:44] it screen be able to be done by a screen reader because right now it can't but they do have the video and so there are things and it also has social media look i did the social medias
[125:04] i was very excited about that so yes next is let's uh conversations contacts see where's forms tickets on missions
[125:30] uh lead capture forms not really a lead capture but you know what if that's what works i'm gonna create a form standalone page
[125:43] next next build my own template okay well it doesn't look complicated to set up so i feel like i should no um i actually don't have a discord but if you want to come hang out
[126:00] on the discord i hang out at it is somewhere let's go look at twitter because i don't remember what it's called go search open source raid guild this is where i hang out and
[126:22] yay yay okay so here you know what i do not disagree with you hubspot isn't amazing but it is
[126:44] something and it is um better than what i was doing because uh why do i keep closing my mirror board
[126:57] mirror mirror mirror mirror recently closed oh my gosh sniffles today is i was using multiple tools for all of this like um i was using monday.com for automation
[127:17] and then i was using notion because it was way cheaper but then it wasn't automation and then i had to do scheduling through calendy and then recording stuff and then producing stuff
[127:28] and the marketing stuff this shit gets really expensive so hubspot at least is like a yes the lesser of all evils i would say of at least i don't have to have hootsuite
[127:45] and uh you know an automation like i can keep it all in the same area i will say that it would be nice if i had something else but like i will use rivet for an example i have nowhere at
[128:04] the moment to say hey i met this person at the denver startup week i should add them and tell me to follow up with them in like a few months because i lose track out of sight out of mind
[128:19] it happens not my favorite feature but it happens and that is a big reason that i wanted to go with um something like hubspot because i wanted to be able to be like hey jen you added somebody
[128:34] you haven't talked to them in a while um or hey jen you had this guest on the show follow up with them or hey jen you had the podcast episode you should probably
[128:47] send it out again because i don't know something like that i want to be able to set up those automations so it's not a manual process because me doing it by myself where
[128:59] companies like have entire teams to do what i try to do and it's um it's a lot for one person so the hubspot is it i'm going with it for now just knowing not to sign any contracts you know
[129:19] nothing long term be like let's let's see if we get along first let's let's see that i will say one tool that i absolutely love that i i won't give up anytime soon is canva it does have its
[129:30] limits but as a content creator it is way easier and faster than um like photoshop or something so canva is definitely dope enough about tools though all right y'all come back i will post
[129:54] on linkedin and twitter if i decide to stream in the next two days i leave on saturday for portugal and will be gone for a week and a half and then i'm emceeing uh what am i emceeing forge
[130:09] nation which is view and next nation um forge nation is actually i should show you guys this nation i will put this in the link here soon
[130:37] viewjsforge.com it's free conference if you guys want to come hang out it's fun i can emcee it i can talk to everybody uh and it's organized by view school
[130:51] oh yeah for sure it is uh my name uh down there if i'm pointing in yes dude join it definitely has a lot of things to learn from and i love i would say let's see
[131:12] i've done view nation and next they should know and just like the team at view school and the entire like view all of just the community is really cool i i haven't gone into as deep as
[131:32] like if i want to do like react or view or like where or svelte or something like that i do really like typescript but that's something that i can do i'm pretty sure on any of them and
[131:46] it's kind of just uh i need to wait and see which which i'm gonna do so i know doing things with astro though i haven't necessarily needed to figure that out
[132:02] but i will eventually i don't know when but i will probably end up using view because it's also i feel like community really helps build interest and that is one thing i really love about the
[132:19] view team and all the people's knowledge so all right y'all i will see you again and have a and have a wonderful day night wherever you are and thank you oh y'all y'all i almost didn't read
[132:39] what is this bananas this is bananas i almost didn't read you guys well we'll raid theo he'll have some hot takes for everybody
[132:53] some spicy takes it'll be amusing all right bye y'all what why does it always take forever i always forget this i'm always like so awkward at the end thank you for joining
[133:13] [BLANK_AUDIO] 
