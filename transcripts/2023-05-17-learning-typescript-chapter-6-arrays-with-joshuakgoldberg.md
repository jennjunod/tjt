---
showLink: "https://www.youtube.com/watch?v=E1UmLmq-bt0"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "learning-typescript-chapter-6-arrays-with-joshuakgoldberg"
title: "Learning TypeScript Chapter 6: Arrays with @JoshuaKGoldberg"
publishDate: "2023-05-17"
coverImage: "https://i.ytimg.com/vi/E1UmLmq-bt0/maxresdefault.jpg"
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

[00:00] humans. Welcome to another episode of TeachGen Tech. Well, TeachGen TypeScript. Hey, it's still TJT. I dig it. I just got there. Took us enough episodes for me to put two and two together.
[00:13] Yet, hello, and we're learning TypeScript. Chapter six of Josh's book, Learning TypeScript, the book. And Josh, who are you and do you want to tell us a bit about what we're learning today
[00:30] with Arrays? Yeah, real excited. I like the energy. This is good. This is high intensity. The difference between a Monday stream and a Friday stream. Hi, everyone. I'm Josh. I'm the
[00:44] author of Learning TypeScript, a book published almost a year ago now by O'Reilly about learning TypeScript. I know, it's wild. I also do general TypeScript stuff. I'm a full-time independent
[00:56] open source maintainer. I work on TypeScript ESLint, which is the tooling that lets you run ESLint, prettier and similar on TypeScript. It is neither TypeScript nor ESLint. Very confusing.
[01:06] And in general, I work on open source stuff in the JavaScript TypeScript ecosystem. And I also really like teaching and learning and exploring how people teach and learn. So,
[01:15] I'm real excited to be here. Jen is a fun person to hang out with. Thanks. And I agree, you're a fun person to hang out with too. Or I agree, I am too. I don't know
[01:25] the best way of saying that. But you keep showing up and it's been, holy cow. I think we've been, like we started streaming like six months ago. Yeah.
[01:34] I mean, they're very spaced out. Yeah. The average is like once every two weeks? Two to, yeah, I would say the average I think is every three weeks. The goal was every two weeks,
[01:47] but the average is every three weeks. And I will say that we got to do this really quick of making sure that everybody goes and follows Josh's stream.
[02:02] Yay. Let's see if I did it right. Yay, I did. Thanks.
[02:11] I have to do it off of memory sometimes. And I'm like, there's, I don't know why, but having to spell your whole name out, I'm like, there's so many more letters than normal
[02:20] because I call you Josh. I hear Josh Goldberg from people. And then I'm like, what am I typing? Josh Goldberg was taken. And now I'm Joshua K. Goldberg-Evigor, even though literally no one
[02:32] in real life calls me Joshua, except for people who only know me online for the first five minutes in real life. Yeah. It's a whole thing. Oh, that's so fun.
[02:39] I also have like six different emails because I kept switching. Life is hard. That is fair. That is fair. And since last time, because I went on work, I went on work,
[02:54] I went on a work trip. There we go. I went on a work trip and then you've been doing some travels as well and some conferences. What conferences have you been going to the last
[03:07] month-ish? Last month? Most recent one was Star Trek. These are all great, by the way. I had a thoroughly excellent
[03:14] time at all of them. Star Trek in Columbus, Ohio, which had a show in Guardians of the Galaxy 3, which was very fun. Volume 3. I'm so excited to see that one.
[03:25] It was good. It was good. I've been hit by the Marvel fatigue, but this movie was it overcame. It was good. I sat in the back with like two things of free popcorn and two
[03:34] things of M&Ms and like a cream soda and just pigged out the whole time. It was awesome. I felt gross in a good way.
[03:41] Cream soda when I was eight. I don't know if anybody else has this. When you're a little kid, you do something really dumb and it scars you for life. That was me and cream soda and
[03:52] grape jelly because I had root beer, cream soda, and grape jelly sandwiches, multiple of each. I think you can see where that might lead and why I dislike them so much now. But all right,
[04:06] what was the next conference? In reverse chronological order, it was React Miami, which was in Miami, in Miami Beach, which is just a beautiful location filled with beautiful people.
[04:18] Upsettingly beautiful, but it was a great conference also. I really enjoyed it. It's cool. It's interesting seeing the two types, like the two common types of conferences.
[04:30] RM, if I can call it that, Miami was a single track, so it was a bit more curated. There was a real story being told, like an alternating, a wave of technical, non-technical, React.
[04:42] Oh, that's cool. Yeah. Whereas, Star Trek was multi-track. There were, whatever, five, six at a time,
[04:49] I think. You could pick and choose and make it more of your own conference. There were a lot more speakers. It was cool. I like both. Yeah. That's something that JavaScript Jam was talking
[05:03] about last week of when you have... Do people like the big conferences or the little conferences? But so many different options. So many different options.
[05:13] I think I saw the JS Jam people there, unless I'm mistaking them for other people at React Miami. Maybe I am.
[05:21] Anthony? Anthony. Yeah, yeah, yeah.
[05:23] Yeah. Yeah. I'm like, "Anthony, that is..." I finally got to saying his last name right, Campolo. It's not as hard as it looks.
[05:32] A lot of names are trickier than they look. Yeah.
[05:38] This is true. This is true. All right. So, are you ready to dive into Chapter 6 of Arrays? I am so ready.
[05:49] Sweet. Oh, Anthony's in the chat.
[05:53] Oh, hey. We're talking about you. Oh, hey. Hey. Were you at React? You were at React? Right.
[06:02] React Miami. Right, Anthony? See if I can talk. Oh, yay.
[06:19] Yay. I'm not going to... I'm so jealous.
[06:23] Yeah. I hear Render is going to be amazing. I also... Going to be in Greece.
[06:28] Oh, so sad. So sad. Yeah.
[06:34] Woo, is me. Visiting Santorini at the... I am going to have a birthday and be hanging out with my fam here. And then we're moving.
[06:49] So, I'm basically just packing the next month and a half. And I'm like, I'm okay with it. Because there's lots of fun adventures coming on later this year.
[06:56] That's actually exciting, though. What's the story with the move? Are you looking forward to it? I... So, the move. I'll find going into this, I think a lot of people have wondered.
[07:10] I am moving. So, currently, I'm in Denver, Colorado in the States. And my partner and I, we moved up here almost three years ago. Two and a half, three years ago.
[07:23] Because a previous job told me, "Hey, you got to move to Austin or you got to move to Denver? One or the two." We chose Denver. And now that I no longer work for them, I'm fully remote. My partner,
[07:36] he can be fully remote. We were... We haven't... There's a good startup community here. And I love the startup world, like Denver. Startup Week is so fun. And yeah, all of our closest friends
[07:49] are in Phoenix. His family's in San Diego. My family's in New Mexico. So, Phoenix is just like the perfect in between. And what I'm getting more excited about is convincing him that we need a
[08:03] pool. This is what I'm excited about, is a pool. I don't know if it's actually going to happen. We're going to rent and he goes out at the beginning of next month and a couple weeks to
[08:16] go look for a place. But fingers crossed, we're going to get a pool. - Good luck.
[08:21] - So, if anybody's coming to hang out in Phoenix, I'll be in Phoenix starting in July, where it's some of the hottest months. And monsoons, monsoons. I'm very excited for monsoons.
[08:32] I love monsoons. - Sorry, monsoons, like the weather phenomenon common in South India?
[08:39] - Yeah, they happen in Phoenix too. - What?
[08:43] - In Tucson. - What?
[08:44] - Yeah. - I don't believe you.
[08:46] - So do Haboobs. - So do what?
[08:50] - I don't know. Haboobs. - Wow, this is... I'm being disrespectful. I should believe you when you tell me pieces
[09:05] of information about the city you're moving to. Wow, I did not know there were monsoons in Phoenix. - Or what a Haboob is. Dust storm. Why is there a region that has both dust storms and
[09:14] whatever a monsoon is? Whatever you classify that. - Heavy rain?
[09:19] - That's wild. Heavy rain, yeah. - Because it's a desert. So the dust storms are because of the desert, but so is the heavy rain.
[09:28] It's like once a year, it gets all of its rain. So you think kind of like a, you know, I don't know. You see in the movies that the deserts only get like so much rain.
[09:38] - That's so cool. - It's like it doesn't happen all year round and then suddenly it like floods.
[09:44] And that's my favorite part of moving back to Phoenix. I'm from Phoenix. So I've been dreading going back because it is so hot. And I think I've been told, multiple people have told me lately
[09:58] that it looks like Mars. I'm like, you know what? That is a really good explanation. - I love it.
[10:06] - It was actually my friend from Germany that told me that it looks like Mars. She is from Munich. So that's a good call. Yeah, they don't really have too many in Germany that I've seen. I'm
[10:23] looking up, y'all need to go follow this human who takes amazing photos of all the lightning and monsoons in Arizona. Like the real beautiful, amazingness photos.
[10:43] I would highly, highly suggest following them. But yeah, that is why I am moving back to Phoenix. And, but this does mean I get to go to the ocean more because San Diego is not that far away.
[10:58] And I'm excited about that. Okay. Enough of me distracting us because I'm like, talking about the fun things. I should, I should talk about the, you know,
[11:10] the part that I'm excited about, but I'm like kind of like, 'cause it's hard. And I feel silly when I do these. Like the more I know, the sillier I feel.
[11:23] Like I should know better is kind of what happens, but y'all, what up Bakari? Hello, beautiful human. I haven't seen you in forever. I am going to copy and paste Josh's
[11:39] website. Well, Josh's learning TypeScript website here. This is where you can get the book and look at all the projects and the articles and like where to get started with multiple options.
[11:54] And my watch will try to say something to us. Watch is very excited about TypeScript. Yes. Socrates is very correct. I know, I know. I'm so excited. I'm actually doing this talk.
[12:12] I'm giving a talk because of Max in two weeks. Well, not because of Max, but kind of because of Max, because Max asked the question that a lot of people have asked me and it stuck in my head on,
[12:24] like, how do you disclose neuro, like neurodivergence or mental health during the hiring process or to your manager, or how do you talk about it at work?
[12:37] So I'm going to give a talk about it. And I'm excited because I feel like it's also something that this show has taught me a lot of is how to learn in my own style, which we're lucky because
[12:54] Josh comes on and talks to me about all this random stuff. All right. We're going to go to the book because I have the book on my iPad and that I'll be sharing. And yes, this week is a
[13:10] raise. And I really appreciated that. Josh, I asked Josh beforehand if he could provide like a bit of information on what do we already know or what is like, is this a new concept or a building
[13:30] concept? And this did help a lot. I will say I still got stuck on some of it, but hey, we wouldn't have much to stream if it just all of a sudden clicked. I mean, I would like it to, I really
[13:47] would, but that takes time. That does take time. Okay. So as we said, this one is about a raise. It's chapter six and I have a little pointer. Let's use the pointer. Yay. I have a pointer.
[14:05] This is fun. This week with declaring a raise and retrieving their members will be about declaring array types with the square brackets, using parentheses to declare array functions or
[14:23] union types, how TypeScripts understand array elements as type of the array, working with spreads and rests, declaring tuple, tuple, tuple? >> I don't know. I normally say tuple
[14:41] and I've heard people say tuple. >> Okay. Tuple, tuple types to present fixed sized arrays and using type annotations or as const assertions to create tuple, tuples.
[14:57] What? I'm curious and for those who have been watching the stream for a while, feel free to tune in of what do you think I struggled with the most this week for this
[15:14] chapter? Or what most people struggle with. It doesn't have to be me directed, but based on the summary. >> There are two kinds of people
[15:22] here that come to mind. One is folks who already have core JavaScript fundamentals down, like really down. And there are people who are like learning this along with JavaScript.
[15:31] I hope both of those were kind phrasings as they were intended to be. >> They are. It makes me giggle. >> I learned from last stream.
[15:38] I think for folks who don't yet have JavaScript down pat, like the dot dot dot spreads and rests, I have found to be a little confusing or hard to go around with. I personally struggled with them
[15:50] when I first learned them. And then for both, tuple types are like a mind meld. Unless you're someone like Max, very nice, who knows tuples from another language. The concept of a fixed
[16:01] size array in the type system, it's just like a lot of things at once for some people. Again, myself included. I think I'm just projecting here the stuff that I personally found more difficult
[16:10] to learn at first. But I love these concepts now. And after having worked with them a bit, I came to really appreciate them and understand why they're useful. So I hope that's you as well.
[16:24] >> Okay. So we were saying working on spreads and rests and basically the last three. And I feel like I was 2.5 understood the top three. And then there was like the very last part of
[16:46] that. That I was just like, I don't know if I get it. I don't know if I get it. >> Oh, that's right. Because it's like the whole interaction of like union types. And
[16:56] if it's like multiple possible things, it's a union of all them. Union types tend to trip people up. Let me rephrase. Union types are something that keeps showing up. So it's one of the concepts
[17:06] that you in particular aren't clicking as well with compared to others. It can keep not clicking. But one of the nice things about it is that because it comes up so often, a lot of people
[17:17] don't realize by the time they get to the end of the book, even if they're like only two-thirds caught up, they have now gotten like two-thirds of a book worth of union types. So going back to
[17:25] the beginning, it's like amazing and obvious and clear. All right. >> Yes. And Max just asked, is there something like array comprehension in TypeScript and JavaScript? >> We talked about
[17:41] like the Pythonic thing. Like array equals for X in other blah, blah, blah. It's been a while since I've done Python, but I remember there being some really cool stuff. >> I gave up my Python
[17:54] streams because I had to kind of just like narrow down on a language and then narrow down on like, you know, does it work? And that and databases like just are absolutely fascinating to me.
[18:08] And then like having a day as like extras. >> Yeah. >> Array equals list or not. >> Yeah. So in Python, they call it lists in JavaScript and TypeScript. We call it arrays. Yeah. So we don't
[18:20] have like a built-in syntax for these awesome comprehensions the way Python does, but we do have a lot of nice comprehension E or functional E methods like .map, .reduce. Now we have newer
[18:32] ones like .flatmap. So you can get a lot of the way there, but it's not as beautiful and clean as Python, unfortunately. >> And what would you call those again? Would you just say they're
[18:45] array types? No, because we go through array types. >> Like list comprehensions is the Python feature, which doesn't really exist in JavaScript. So like there's no equivalent term. >> Okay.
[19:01] Okay. That's fair. That's fair. So these ones didn't have a lot of examples. I just highlighted some things that if I needed to look back into this that I thought was helpful, which was
[19:13] TypeScript respects the best practice of keeping to one data type per array by remembering what data type initially was inside the array and only allowing the array to operate in that kind of
[19:29] data. Wow. >> What a sentence. The fact that you're tripping up on that is reinforcement for my personal opinion that that's not a very good sentence, that I should have split it into like
[19:38] two or three sentences from just like an editorial point of view. >> Well, for me, I get TypeScript and respects and then data and then array. Like they're words that I just kind of
[19:53] like, but I also stumble on my words a lot too. And I really liked during this, and we went over this example showcases that we used the array that had two strings. So it wasn't going to
[20:10] let us use a Boolean to do it because that Boolean wasn't put as a string. If it was true in parentheses, it would have worked, but since it wasn't, it did not. Voila. Y'all, I feel very
[20:28] excited because like two chapters ago, I would not have gotten that. And yes, this was just, again, just saying that it tries to guess what you're going to do and make sure that it understands
[20:43] what you previously did to help you with that. And that made sense to me. Array and function types, array types. And that's why I was like, oh, wait, we didn't really, it wouldn't be the same
[21:02] as the comprehension, array comprehension, because we do go through array types. And it's with the, I'm not seeing the, oh, what's the big difference here? I guess I should ask that as a way to
[21:25] maybe have you explain it for the parentheses types. >> In general, there's parentheses, you're talking about array and function types, just to confirm?
[21:40] >> Yes. >> In general, this is just us telling the syntax things the right way. The first one of those two things is a function
[21:52] that returns string array. The second is an array of things, where each of those things is a function that returns string. We're using parentheses to indicate, like to change what it
[22:03] means. Because if we didn't use parentheses, we might be telling it the wrong thing. Which shows up in code a lot, right? Like having to use parentheses or semicolon or something to indicate
[22:13] when it's not very clear what it could be. >> Yeah. Okay. That made a lot more sense. Thank you. Union types, I mean, arrays, this actually started making sense. And I was excited
[22:26] about that. And I still go back to the original way of saying it. But it makes so much more sense on being able to take two different types and make them friends. That's how I've been
[22:40] explaining a union. >> Cool. Yeah. >> And making them friends. And then I figured out how to put an emoji on this. And I was really
[22:52] excited. But I was like evolving in any array. And I'm like, why is this not clicking? Like, I get when you would use any. And because you don't know what you would actually do. And then
[23:05] normally you would go back and change it. But I don't necessarily get how it evolves. And from here I kind of just -- it wasn't sticking. >> That's fine. Do you remember how evolving
[23:20] anys work with variables by any chance? The answer will dictate which of two potential things I use to explain approaches. >>
[23:32] Yes. Because if you did an any with a string, then the next any and you try to Boolean, it wouldn't like that one because you previously used a string.
[23:45] >> Sort of. Can I show my screen? >> Yes. >> Futs around with the Zoom settings. Window. Type your playground. Okay.
[24:01] So, let's say we have a variable. Let value. And we say value equals hello. From line 3 and onwards, we know that values type, which I'm looking at using this little
[24:12] two slash comment, just like a nice little editor utility. We know that it's a string after this point. Does it make sense why TypeScript thinks value is a string here?
[24:21] >> Yes. Because it was value equals hello, which is a string. >> Yes. But before we said value equals hello, we don't know what type value is.
[24:32] So, TypeScript is like, well, undefined. This is something called an evolving any, where you're allowed to put whatever value you want in it. Because you never actually said
[24:45] originally what that value was going to be. But this is totally okay to first give it a string and then give it a number. Does it make sense why TypeScript allows that?
[24:56] >> Yes. I guess. It's almost like and hello. It's almost like I feel like it's contradictory. Because if it's going to allow you to do any, or let it be evolving, then you can't
[25:26] how is it going to learn if you can continue doing it multiple? >> You bring up a good point. Also in the chat. Sometimes people put in different things in a
[25:41] variable. Like that sometimes. You can do that in JavaScript. But this is not good practice, I would say. Depending on the situation. In general, you probably want to put an explicit
[25:52] type annotation on something so that later on if you change its type to something different, then TypeScript will yell at you. But if you don't give it a type, TypeScript's just like,
[26:04] whatever you say goes. I'll just change it to whatever you say. So, again, I'm not saying do this. I'm saying this is a feature of the language for the case
[26:12] when you don't add a type annotation or default initial value. Does that make sense? >> Okay. Yes.
[26:22] >> Eh. Cool. Let's look at arrays. Let's say we have values equals empty array. We do values.push hello. Then we look at the type of values. Now it's a string array. It's the same idea.
[26:40] Values started off as I don't even know. Was this never or something? Okay. Implicit any. Let me turn that off. There we go. So, TypeScript actually has some
[26:55] options to complain in cases like this. But, yeah. So, this is an evolving any array. I forget actually what it's called. But here we start off with an empty array. And TypeScript
[27:05] has no idea what's in the array. So, it says, like, never or any or like some default type. And then as soon as you add something to in theory, it should not be yelling at us. In
[27:17] practice, it is. You know what? My book might be out of date. Maybe it's wrong. Let's find out. You're now watching me relearn this stuff in real time. What page are we on?
[27:34] >> We are on page 77. >> 77. And my browser is freezing. >> Or 103 in the PDF. >> So, page 77. Come on, browser.
[27:56] There we go. So, when we start off okay. Yes, yes. When we start off with this empty array, TypeScript doesn't know what goes in it. >> Are we supposed to be seeing more on your screen?
[28:08] >> Yes, we are. Sorry. I'm sharing the wrong thing. Chrome is freezing. Love to see it. There we go. Okay. >> Do 103.
[28:24] >> Found it. There we go. So, type any. When we start off an empty array, TypeScript doesn't know what's in it. But if you add something to the array, we push string. TypeScript knows, okay,
[28:39] this is a string now. And then later on, if we assign something else to the string, to the array, if we set values of 0 equals 0 or dot push 0, TypeScript will evolve its understanding of the
[28:50] array. It knows that no longer is it just strings. It's also numbers in there. So, number or string. And that doesn't make sense. So, it learned that by doing two
[29:08] but so, would it keep learning if you did let values equal empty array and then values dot push equal hello, then values in the square brackets equal 0, and then if I say values dot,
[29:32] I don't know, Josh equals true, then it would add a Boolean into the array? >> If you did values of 1 equals true, then yeah. Yeah. It would add a Boolean to the type. Because
[29:48] it would know that, okay, in addition to previously knowing that this can contain number or string, it can now also alternately contain Boolean. Which is not, again, this is
[29:59] similar to evolving any variables. This is not something you want. This is weird behavior. And I honestly debated whether to even put it in the book. Because you should never do this. But it's
[30:11] interesting if you end up in this situation, I think. >> Okay. Anyone else have questions for that? I'm gonna switch the share screens just in the meantime. Because this is the part that we
[30:30] were at of and I'm gonna work on summarizing it. No. Okay. Fine. There we go. Go away. >> I'm also finding that when I try this out in the TypeScript playground, it's not actually
[30:45] working anymore. So either they updated something or my book is inaccurate. Either way, I don't think this is very important information. >> I'm just gonna say meh. We'll just do meh.
[30:59] But so that way I remember is when we added a string, it became okay. It makes more sense now. I guess I don't really need notes. It just made more sense actually going through it than just
[31:13] looking at it. So thank you. But yes. You are accurate that as soon as we went into the new stuff, at the very beginning. So okay. First off, I don't feel as bad about not understanding any
[31:29] arrays now. Because well, they seem kind of complicated. And yes, they are referred to earlier on. But it doesn't seem as like out of like I don't know. I was like why don't I get it?
[31:44] We've gone over it. But it also makes sense. Yeah. Then we go to multidimensional arrays. And I'm like I don't necessarily know where to start or kind of could you tell us more about this section
[31:59] and more detail, please? >> Sure. So there's no new theory introduced here. It's just showing using the same thing twice. What it's showing twice is
[32:11] indicating that there is some type with the array brackets next to it. Twice. So we have a number array. So an array of numbers. And then we have an array of that. We have an array of arrays of
[32:23] numbers. Thoughts? Also high-technology depth also. >> Yes, hello again. Max has a question for you, Josh. I'll let you two discuss that while I like stare at this
[32:50] for a second. So this does make sense. I think where I'm at for it, though, is here let me move that over. Oh, hey, this is how I should do it every time we're streaming. Look at this.
[33:17] This is like great promotion for the book. Okay. Go over there. Would this be almost expanded on the evolving one? Because the first one that we have right here is just having it in the brackets
[33:46] and then this one is having it written out. >> Sorry. Could you repeat that? I'm not sure I parsed it. >> So and I think it's because we
[34:01] just talked about the any or the evolving ones. This is another reason I'm a little stuck. So we have let array of arrays of numbers be number in the two brackets. And then array of
[34:16] arrays numbers equals brackets of numbers within the brackets. So is it evolving? Like the previous one was because this first one is empty. So it can be anything. But the second one actually is set
[34:35] This is not evolving. These are totally separate things. The concept of evolving is when you don't fully fill out the type and there's these very specific situations where TypeScript will allow
[34:45] the type to change over time. This is a type that's known ahead of time and never changes. And the type just so happens to be an array of arrays. >>
[34:53] Okay. It's starting to make sense just to verify of if it were and going I'm pretty sure is like if it had let's say a 4D array, it would still be
[35:21] that's a 2D array. >> This is a 2D array. You could have a 4D array. You could have a 100D array in theory. Just arrays of arrays of arrays dot dot
[35:33] dot. >> And would they all be within each other or would they be next to each other? >> It would be number array bracket array
[35:41] bracket array bracket and so on and so forth. >> Okay. Okay. It makes enough sense that when I get to it later on, I can go back and mess around with it more because this is connecting
[36:01] a bit more now. I think I did get stuck on trying to put it like the previous one. Yes, they are different sections. But yes. Can you put arrays into arrays into arrays?
[36:12] >> You can. You could have array section. Yo, dog, I heard you like arrays. Whatever meme/internet reference you like for deep things within each other. Yep.
[36:23] >> But that one wouldn't be called a 2D array because the 2D is just next to each other. So and the 4D are next to each other because if it was like a 4D, it would just be number
[36:36] and then bracket. Bracket. My really bad drawing. >> Each array has a dimensionality. That's like a way to think of it. Like most of the time you're doing 1D arrays. It's just an array of stuff.
[36:53] When we call it 2D or two dimensional, it's referring to the idea that it is an array of things that have that dimensionality minus one. So a 2D array is an array of 1D arrays. So in
[37:05] theory you could have a 9,001D array which is an array of 9,000D arrays which are each arrays of so on and so forth. So nesting is another way that we call this. This is a nested array of numbers.
[37:17] That term works well for others. >> Thank you, Ryan. It's evil, though. Okay. But that did help. That did help. Thank you.
[37:35] Nested for some reason made more sense in my head. But okay. And then we go to array members. And say what? >> Yeah, this actually I regret
[37:53] a little bit. I remember going over the fence of whether to call things array elements or members. I think I switched to element over time, but kept something as members. So you have an array of
[38:03] things. So an array is like a big list of stuff of some size. 0, 1, 59 million, and 1, whatever. Each of the elements of those arrays sorry, each of the elements of that array is a thing of that
[38:19] array's type. For example, if you have a string array, each element of the string is sorry, each element of the array is a string. Defenders of 0 is type string.
[38:29] Before we move on to unions, does that make sense and sound reasonable? >> Yes, because that did make sense of why it would be I think elements make sense a bit more.
[38:46] >> Okay. >> Sometimes and for if anybody's curious, I love hate that you can have different names for everything. Because especially
[38:58] like an argument is not the same as it is in the English language. It means something completely different. And it's like, wait, let me have a similar word so it doesn't associate in my head.
[39:13] Yes. Yes. Okay. Yes. Yeah. Because this is totally making sense. And Max said is then indexing then as frustrating as Python when it's a nested array.
[39:36] >> Yeah. I would suggest so yes, it is equally confusing in JavaScript and Python and C# and all languages to have a nested or multidimensional array. Fortunately, TypeScript does not add to
[39:48] that confusion. In fact, I would say TypeScript makes it easier because TypeScript will let you know if you've gone too deep or not deep enough with your shenanigans.
[39:56] >> I really like that. I really like that. And that's something that I think I'm running into. I've been working on Theo's T3 app, T3 stack app, that thing. And I think, yeah, I think I ended up
[40:18] nesting something a bit much. And now I have to figure out where I put the error. And TypeScript is telling me, well, yeah, it tells me there's an error, but then I can't, this is some of the fun
[40:31] of learning things is you don't always understand, is this a CSS error now or an actual TypeScript error? It's fun. It's learning, y'all. It's learning. All right. Caveat. I'm going to
[40:44] unsound, I'm going to put elements because for some reason that word makes more sense to me. So if I put that in there, it's like saying,
[40:58] this code gives no complaints with the default compiler settings because this is a string. Elements is a string with the brackets. So therefore it's saying whatever you want in the
[41:11] string. Can you go into a bit more detail here, please? >> Sure. Oh, let's talk about the concept of a type system. A type system is supposed to let you know when you access something that doesn't
[41:29] exist. Let's say I create an object which has the members, I don't know, first name, last name, and then I ask for object.middle name. TypeScript's type system would then yell at me saying, ah,
[41:40] you never said there was a middle name. Does that sound reasonable? Cool. So let's talk about arrays then. Arrays, you access some arbitrary number to access the elements or numbers. You can say
[41:54] elements of zero to get the first one. Now we have a problem. Because what happens if you just say it's an array of whatever size, let's say string array, you don't even know what size it is,
[42:05] and then you ask for the element at position 9001. TypeScript has no way of knowing whether there are 9001 elements to get, you know, whether there are 9002 elements in the array or more.
[42:18] So this is a flaw in the model. Either TypeScript is overly pessimistic and yells at you saying, ah, you never said there was 9001, which would be a real pain in the butt, or TypeScript is just
[42:28] like, ah, it's fine. I assume that that element exists. Which is a problem because as we see in this little code snippet, the four lines of code, we're providing an element, an array as an
[42:40] argument that only has two elements. And then we're asking for elements of 9001.length, which doesn't exist. That's going to throw an error. >> Is it, although, is it seeing that 9001,
[42:54] it's like unable to do the length because, yes, it doesn't know if it's actually a thing, but is it because it was said to be a string and not a number? Does that have anything to
[43:08] do with that? >> It doesn't. All we're saying is that we want the 9001 element of the array and TypeScript is not going to yell at us because TypeScript doesn't know whether there are 9001
[43:19] elements in the array. So even though this code type checks just fine, it will crash at runtime, which kind of is upsetting because TypeScript was supposed to prevent that.
[43:28] >> Let's see if I can actually get it to copy. Copy. I'm going to say TypeScript doesn't know. >> Paste. Yay. That was fun. Yes, we're taking a drawing moment.
[43:52] >> Drawing moment. Yay. Okay. Cool.
[44:24] Spreads and rests. Spreads and rests. >> By the way, I should note TypeScript does have a compiler option that makes it more strict around element accesses. It's
[44:47] no unchecked. I never use it because it's real annoying to work with. It's no unchecked indexed access. It will make sure that if you ask for an element of an array at a particular index,
[45:00] you did something to make sure that index exists. Like checking if the element's length is greater than 9001. Almost no one uses this because it's real annoying. So this is just a flaw in the type
[45:11] system we all live with and hope for the best. And I'll paste a link in the chat. >> Cool. Thank you. Cool. Okay. >> All right. Moving on. Anyway.
[45:34] Spreads and rests. This is very much a JavaScript thing, not a TypeScript thing, but TypeScript does recognize these things. >> Okay. Remember rest and parameter functions
[45:47] from chapter 5. Rest and parameters. And array spreading both operator and key interact. Oh. So summarizing spreads, is it just saying what you can create the arrays with an input?
[46:21] >> Yeah. In JavaScript, you can spread or mix and match arrays together. So if you have an array of strings and you join it with an array of numbers,
[46:34] the result is an array of string or number. Voila. >> Okay. >> Why is that not a union? >> It is a union. It is an array
[46:52] where each element is union string or number. You're right. >> Okay. But it's like I guess it's weird because it's another term for it. But yay. >> There's no new term here. TypeScript. So
[47:07] there's the JavaScript terms of spreads, let's say we're looking at. And then there's the existing TypeScript terms of array elements and union types. And this is just matching those all together.
[47:17] >> Ah. Okay. >> So
[47:49] apparently if anybody ever does read my notes from your book, they're going to be like, why is everything making friends with each other? Like is that like the new thing in coding,
[47:59] like making friends? Yes. It's going to be my answer. Okay. So spreading rest parameters, I'm going to reread it now with that context because with spreading.
[48:12] And you're right. I think it is because I'm not used to the terminology in JavaScript either. Yet. Yet. >> Yet. >> Spreading an array of types string but
[48:42] is loud but not number is not. So is it saying spreading rest parameters because it's saying that we can do it with strings but we cannot do it mixing the two? >> Yeah. It's not specific to
[48:57] strings or numbers. It's just in general the log warriors function says that the names must all be strings. But then we're providing numbers. So that's a type mismatch. Same as if it was just
[49:07] the one argument, let's say greeting is the parameter, say string, and we tried to provide a number for it. >> So it's like the opposite of spreads.
[49:19] >> Because spreads let us combine the two, putting numbers and strings together where this one's like no, bro, you can't do numbers in our strings. >> Yeah. Sorry, you said spreads,
[49:35] but I think you meant spreads. >> Oh, sorry. Yes. Yes. Yes. Yes. Cool. I -- yeah. I like -- I personally like to think of spreads and rest in that way,
[49:52] agreed, plus one, that it's like the opposite. Spreading joins them together and rest are a way of like getting that join. And then -- >> Right. But like why is spreading like
[50:03] putting them together? Like that's -- that's language. Me in languages, not me in disagreeing with you. Language. Language. >> We're taking an imprecise medium,
[50:13] the human languages, and then trying to map it to a precise format programming and it's never going to work well. Yep. If only -- there's -- by the way,
[50:23] there's a cool language project called Esperanto where people tried to make a language. Hasn't caught on worldwide, but eventually maybe. >> Wait, they're trying to make a language what?
[50:35] >> Sorry, this is like totally random and tangent and probably harmful to the stream to bring up to distract you with. But there's a cool project called Esperanto,
[50:44] which is a language that people made. It's like -- it's called a constructed language. The idea is all languages suck. Why don't we make a better one? The problem is no one -- no one like
[50:57] grew up -- like no one's ancestors spoke Esperanto, so. >> Oh. Interesting. Oh, it was banned? Oh, yeah. It was like Jewish -- banned in World War II by Hitler, so not the most modern, you know.
[51:15] >> Oh, okay. >> Don't worry. >> Oh, there's a beginner's guide, but it's from like 2000 -- oh. This one's from 2023. This one's
[51:28] from 2003. But let's go with Britannica. I didn't realize Britannica was still a thing until like two weeks ago. Y'all, I want to make friends with Britannica again, because they also just have the
[51:44] play button right here, and it's like, okay, cool. I'm going to share this link, because it's Britannica, and I want to go look into this language later on. Oh, how cool.
[52:03] >> Relatively -- these words are derived from -- >> Huh. Huh. Okay. I will look into that more.
[52:13] For the word we can't say, tuples, tuples, wupples. >> Mm-hmm. >>
[52:36] I'm still confused why these aren't like just different ways of saying unions, because now that I'm finally starting to get unions, I'm like, but it's putting two together.
[52:44] >> Forget unions. In theory, we can like mix and match the two concepts, like you can have a union and tuple, but for now, just forget them. Tuples are on their own, very separate. Sound good?
[52:55] >> Yes, in that context, could you go through tuples, please? >> Everything in an array is -- like in the arrays we've looked at is the same type. We said it's
[53:08] like an array of strings, so all the elements or members are strings. Does that make sense so far? >> Mm-hmm. >>
[53:14] In a lot of modern frameworks and libraries, that's not the case. Like in React, it's very common to call a function that returns something that is like an array of size 2, where the first
[53:27] thing is like some value and the second thing is like a function that takes in that value or something like that. I forget, have you played with hooks, React at all?
[53:35] >> No, not yet. I've played with some web hooks, but I don't think those are the same hooks you're talking about. >> Not the same. Same root concept of hooking
[53:49] into something, but yeah, not the same. So if you don't mind, I'm going to share. Okay. So let's say we have a function that's like get count and updater.
[54:00] And we have let count equal zero, and every time someone calls us, we return count and a function that increments counts. So like const count -- here we go. Let's say -- I'm like trying to
[54:29] construct a good example here. Okay. So like function main whatever. So let's say hidden counts. There we go. I'm writing some code that has no type annotations intentionally,
[54:45] because this is just JavaScript code. So count, increment count equals get count and updater. Log count. Then increment count, and then we again console.log count.
[55:01] And you know what? Let's just pretend that that's not yelling at us, because TypeScript. So if we run this code, we get -- nothing, because I forgot to call main. I don't know how to code.
[55:14] If we run it, we -- updated count equals get count and updater. All right. Here we go. All right. One last time, I'll just run it. Okay. So this function returns two things. An array containing
[55:36] two things, two elements. The first thing is a number. The second is a function. So far, up till now, prior to tuples, we have not had a way to represent this
[55:46] well in the type system. Because right now, TypeScript thinks that this is a function that returns like a union type of number or function that returns number as the array elements. But
[55:58] that's not actually right. This is returning -- it should return number and function. Does that make sense? >> Yes.
[56:09] >> Like why TypeScript is wrong here? >> Yes. >> Cool. Actually, you know what? I'm sorry. I just realized there's a better way of explaining
[56:16] this. Let's say I'm called and math.random happy or sad. So let's like count and emotion. Here we go. So first count and first emotion. Sorry. I normally try not to take this long to get to the
[56:44] point. But I just realized my point wasn't well made. So here we go. The reason why I like this more is because we're not messing around with functions. We're now talking about just strings
[57:00] and numbers, which I find to be easier to understand. I don't like having to bring in functions. Okay. So it's not that this thing returns -- this function returns an array of
[57:10] string or number. What we want to know is that it's returning an array where the first element is a number and the second element is a string. Because I want to be able to do dot to uppercase
[57:20] on my emotions. Because I have very strong emotions. I don't know about you. And TypeScript isn't letting me do this. Because even though we humans can read this and know that the JavaScript
[57:29] is valid, TypeScript's like, ah, but what if first emotion is a number? So that's why TypeScript is wrong so far. Does that make sense? >> Yes. Yes. And the fact that I'm going to have to noodle
[57:48] on it. It's making enough sense. But if I were to try to say it back to you, I'm not there yet. >> Okay. So the problem is that when TypeScript sees an array, it infers the array's type to be
[58:04] a union of all the possible things in that array. So this thing's inferred type is string or number array. Because -- I'm just going to call it number or string because I like alphabetical order and
[58:15] that's the actual order. This is a number. This is a string. That's poopy. What we actually want is to know that it's -- oh, that's no good. What we actually want is to know that it's, like,
[58:29] actually an array that has two elements in it and the first one is a number and the second one is a string. And if we were to use that as the return type, then TypeScript would know that first emotion
[58:41] is a string and thus has two uppercase. And thus we see the concept of a tuple, which is more specific than array. Similar to how, like, literals are more specific than primitives. This is an
[58:53] array that contains not just generally numbers or strings, but specifically the first element is a number and the second element is a string, which makes TypeScript, much like my emotions apparently,
[59:04] happy. >> Okay. Okay. I am too. I like it. I like it. I'm looking at it now. This is making enough sense. I will say it like that. But also with your explanation of it,
[59:27] it makes more sense why it's called tuples or tuples or however you're supposed to say it, it makes more sense why it's called it. >> It comes from the math. Like, in math,
[59:39] a tuple is like a list of things. So here it's a list of things with, like, a specific ordering. >> But it would always be two things, right? >> It could be any number of things. Technically
[59:52] an empty array. You could have a couple that is just nothing in it. Or you could have number, string, number, Boolean, string array, three or four. It's like any array. You can put whatever
[60:05] you want in there. It's just you're specifying what's in it. >> Okay. Okay. Okay. As I said, I think it's going to be a noodle on things, but it's making enough sense.
[60:21] >> Cool. >> So then that leads into what you were saying on it could be a multiple things, but you would have to assign what one they're going to be
[60:32] like you did in your example. Since it's tuple assignability, you need to tell it if it's going to be Parallels is having Boolean and number. Okay. I think this makes sense. That it was just
[61:06] going into that we need to tell it what they are going to be like what you were just saying on right here. We just need to tell it that it's going to be a Boolean, number, and string. Or
[61:20] it could be a number, number, string. Right? >> It could be whatever you want. Put your favorite data types in there. >> Okay. Then tuples as rest parameters,
[61:38] and this means that there are no friends because they have to be a specific thing. That's what I got from when we did rest parameters earlier. It means they're not going to be friends.
[61:52] >> No, friends. Sad. No, it's TypeScript. This looks in my mind like looking back at this, the code syntax here looks more complex than the theory behind it is to me. TypeScript is letting
[62:06] us know if we might be wrong. When we spread the pair array into log pair, TypeScript is yelling at us because pair array is inferred to be an array of number or string. TypeScript doesn't
[62:18] know that it is specifically the first thing is string, the second thing is number. That's why it's yelling because we might have modified the array between creating it and calling log pair.
[62:45] And also, by the way, I want to reiterate, there is a similar mental model in understanding the differences between literals and primitives as there is the difference between tuples and arrays.
[62:56] I think of literals as more specific primitives. I think of tuples as more specific arrays. So if you mess around with them, if you try to pass the less specific thing in a place that
[63:05] needs the more specific thing, TypeScript might be upset about you not being specific enough. >> Okay. Okay. That's making sense. >> Cool.
[63:16] >> Enough. Uh-oh. Okay. Tuple inferences. >>
[63:44] Could you go into this one a bit more? >> Sure. >> Because I'm going up here, like, starting with, like,
[64:04] TypeScript generally treats arrays as variable length arrays, not tuples. If it sees an array being used as a variable initial value or return value for a function, then it will assume flexible
[64:19] size array rather than a fixed size tuple. And when we're talking about that, it's that we have the function as the input is string, so, therefore, it doesn't know that it can do
[64:42] another input of a number, right? >> I think I lost you somewhere in there, but I believe the gist is correct, that
[64:55] the -- by default, TypeScript won't infer that something returns a tuple. It will infer the more general array type, because it doesn't know whether you want to later modify that array.
[65:08] That's why -- that's why the example we were looking at on my share earlier was upset, because TypeScript assumed it was string or number array, not, like, a tuple with string,
[65:19] comma, number. So, like, TypeScript's inference is kind of vague and not very precise intentionally. Does that click nicely? >> It will. It will. This is one thing that I,
[65:33] like, I wish it did, but, you know, the fact that I got, like, the first half of the chapter pretty well is something I didn't think would happen for a while. What up, Graham?
[65:47] And I feel like that goes into explicit as well. >> Yeah. So, you can -- what we did, what I showed and what you are now seeing is, yeah, you can give an explicit tuple type. You can tell
[65:58] TypeScript, I know you think this is the more general array, but, no, it's specifically the tuple with whatever's inside. Telling it to be more smart. Similar to how sometimes you have
[66:09] to tell TypeScript, don't give me the general primitive string. Let's say, give me the actual literal, like, quote, hello, or whatever it is. >> Okay. And then const asserted tuples.
[66:23] I still don't know. It's such a weird word. I don't know why tuples is weird. So weird to me. Language, apparently, is just weird to me, and I'm excited to look up another language. Graham
[66:40] and Ryan, anybody still hanging out with us? Would you say tuple or tuple or something else? >> I'm looking forward to people saying T-U-P-L-E is the pronunciation in the chat.
[66:52] >> Yes, yes, yes. >> I pronounce it G-I-F. >> Tuple. >> Tuple.
[66:59] >> Yay. We got a tuple. >> Definitely the more fancy sounding. >> Tuple. Okay. So, typing out tuple, tuple. Oh, I like Ryan's. Tuple. Tuple.
[67:21] >> Tuple. That's like a slight variation. >> Can be a pain for the same reasons, typing out any explicit type annotations. It's extra syntax.
[67:32] >> By the way, this chapter is one of the ones that really solidified my opinion that given enough time, the optimal strategy for learning TypeScript for many, even most people,
[67:42] is to learn JavaScript first. Now, obviously, if you don't have the time or if you just want to dive in, you know, fine. But, like, this chapter is a lot easier, in my experience, for people who
[67:50] already have, like, a really good, solid, like, JavaScript spreads and arrests understanding. So that, I think, is why all these new terms are piling up all of a sudden.
[67:59] >> I mean, that's fair enough. >> You're doing great going through it. >> More homework to do. And it's definitely something that, as I've been working on
[68:12] different projects, that it's definitely without realizing it, it's starting to make sense. So, it's something that I'm really enjoying. Because, you know, instead of actually going
[68:26] and doing, like, you know, a boot camp and learning in order, I'm just randomly going off and being like, yeah, I'm just going to try to build this app. Because that looks cool.
[68:35] >> Cool. >> Yeah. And I'm going the harder route. I know this. I know this.
[68:47] It's I wouldn't suggest it for anybody. But it does make it a lot more fun. >> This is definitely more fun. I think a lot of people get hung up on trying to do
[69:01] stuff the right way. What's the perfect way to learn, whatever, open source, whatever, just going in and having a hard time and learning stuff, that's a totally valid,
[69:09] even great way to learn this stuff. >> I break a lot of shit. And I will have to give a huge shout out to Ramon and Jacob and Anthony and Roy and all these amazing
[69:23] humans. Because I literally go, hey, what am I trying to Google? Like, I don't want the answer. I just want to know what to Google. Please and thank you. Which also,
[69:38] Jacob has been really great about telling me that I was, like, on the right track for something. But I, like, missed something minor. So I just kept going. It's like I missed my turn. And I'm like,
[69:53] oh, I'll just keep going. It'll be fine. >> Like in the bad part of town, all of a sudden, this is not where I want it to be. >> Yeah. And this is making enough sense to me.
[70:02] It's just doing it as a const so that way it already knows it. Oh. Hey. Yay. And I always love these are the best part in every single chapter.
[70:28] For anybody that's curious, this is the best part. What's a pirate's favorite data structure? Arrays. Arrays. We're going to have to tweet
[70:43] this out later today because that is a great one. But, okay. We talked about declaring array types. Got it. Using parentheses to declare arrays of function or union types.
[70:59] That one made sense because if we put the parentheses in different areas, it means different things. How TypeScript understands array elements as the type of array. This is
[71:11] where I got mixed up from members and elements. And but it makes more sense in elements. Working with spreads and rests. Now understanding that more. Tuples are going to take me a while. But
[71:29] it makes enough sense. And type annotations or assertions to create tuples. Makes more sense than the tuples themselves, but still need to learn tuples. All right.
[71:45] What do you think we should if is there anything that you think we should have spent more time on in this chapter? >> I think we're fine. Arrays
[72:00] and TypeScript really are a reflection of how they work in JavaScript. I like what we went over. This was fun. This was good. >> Cool. Cool. Well, yay. That means
[72:12] we did it. Anybody in the audience have any questions? Because we'll go into them. Because we have a little extra time. But and then also let me grab all your informations.
[72:31] So, that way we can share it. Yay. Yay. And everyone go follow Josh. I almost said array. I just want to let you know that.
[72:53] >> Follow array. I love array. >> Oh, what's your try one question. We'll see if we can answer the one question.
[73:07] We'll try one. But yes. Josh normally is here every other Friday. But I moved Fridays and I am working on doing things more consistently. We're working on it. We're
[73:24] by me saying myself multiple times of we're. It's okay. I will say like something as a random thing, if Graham is writing out any questions, I will just randomly shout this out to everybody.
[73:39] I am looking for when shouldn't you use a tuple then. But you wouldn't necessarily use a tuple if you need more than one thing and not to define it as closely as you would an array. Because an
[74:00] array is more options than a tuple is. A tuple is more precise. Did I get it? >> Exactly. Yeah, you did. Awesome. See, this is what I mean. No one gets all the little trivia
[74:18] immediately. We're discussing the points. But for you, I think you nailed, absolutely got the core concepts. Tuple is a fixed size array. Or at least a more specific array. Normally fixed size. And
[74:28] then arrays are like, yeah, whatever. It's a list of things. Sometimes you don't want it to be more specific. >> And Kiona is good. Kiona is asleep right next to me on the couch. Chair. >> Appreciate
[74:44] the question. >> Yes. >> There he is. >> Great. Let me just see if I can. Oh, I've disturbed him. You see half of him, I think. That's his butt. >> There you go. I can show you guys what I'm
[74:58] doing after this. Because my office has turned into scary. But I'll show Kiona on the way and then you guys can see scary. Maybe. Maybe. >> Scary is fun. >> Doggo. >> Doggo. >> And scary.
[75:18] These are all, like, clothes I'm going to keep. But I need to put them in the vacuum seal bags. So they're just taking up my entire office. But hey, like, at least my camera doesn't show
[75:31] that normally. That is a good thing. >> To answer the question in the chat, I passed a gem. >> Is this a valid tuple? I'm going back in the book really quick. Just to
[75:51] because it can do more than one. It can do as many. Yeah, because well, yes, but you would have to have the assignability before it with the const?
[76:09] No. I'm answering myself before. Well, yes. Yes. I think so. We're going with I think so with the const. >> I'm sorry for putting you on the spot. But yes, you're absolutely completely
[76:23] right. Both of you. That is a very valid tuple. It's a tuple just to recap. So you're saying that that variable names tuple is something that is an array where we know the first element's a number,
[76:34] the second element's a string, the third element is a Boolean. And then, yep, assigning 25 false to it would in fact be fine. TypeScoop would be very happy with you. >> Yes. Yes. Yay.
[76:47] Graham, I'm glad we were at the same spot. I think so. I think so. And this is, it's definitely something that I would say, I think these, I always get really nervous about
[76:59] these because like, as you said earlier, Josh, about what Socrates said. Let's see if I can, I can't, is it going to let me scroll up enough? Let's see. The more I know, the more I realize
[77:14] I know nothing. That is how I feel. >> It was really funny to me that you quoted that directly without even, you almost said the, I forget what you said,
[77:24] was very similar to this. Yeah. >> Yes. Yes. And I am getting there. I am getting there. And thank you, thank you, thank you everyone for coming to hang out.
[77:40] Make sure you like, and if you feel up to it, subscribe. I need to come up with like cool ideas for subscriptions and stuff. What do you do on your channel, Josh?
[77:51] >> Nothing. People keep telling me I could do more with Twitch and I should, and I don't have anything. I like barely, I once have had like a countdown and that's it.
[78:02] Bang. Someone tell me what to do. >> Yeah. Yeah. I could up my Twitch game. But I also enjoy the way it is because I'm like, it's just so nice. Yes. Yes. There are so many
[78:17] options. I will say something cool that Anthony is working on, if he's still working on it, is looking into something for the Whisper AI, which I'm really excited about because it,
[78:32] I guess it transcribes videos and audio for free, but you have to create an app for it. And I'm like, this could be cool. This could be really cool. It could be a step of many
[78:47] of automating the system. And tomorrow I will be streaming about Postgres and setting up my website more. Maybe. I'm going to be doing database design,
[79:01] so I don't know if I'm going to be setting it up yet, but I'll be doing something. And Josh, anything you want, when's your next stream? Do you know?
[79:11] >> Oh, yeah, thank you for asking. My next stream, I have my normal times this week, so that's 2.30 Eastern on Tuesday, and then tentatively 10.30 a.m. on Thursday,
[79:23] but I might push it back to 11. We'll see. >> Noise. Noise. Well, amazing. And let's see where we're going to go raid today, y'all. Raid, raid, raid, raid, raid, raid, ooh.
[79:39] Coding Garden or Chris Griffin. I really like Chris. I mean, I like both of them, but let's go with Chris. Let's go with Chris. All right, y'all, you're going raiding, raiding, raiding. I don't
[79:54] know why it has a countdown. It always makes it really weird. Why does it have a countdown? I get excited about raiding, and then it takes ten seconds. Okay, bye.
[80:04] >> And you're stuck. Bye. [BLANK_AUDIO]

