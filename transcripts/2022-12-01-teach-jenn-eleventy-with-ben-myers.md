---
showLink: "https://www.youtube.com/watch?v=lYZXKCjkoHk"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-eleventy-with-ben-myers"
title: "Teach Jenn Eleventy with Ben Myers"
publishDate: "2022-12-01"
coverImage: "https://i.ytimg.com/vi/lYZXKCjkoHk/maxresdefault.jpg"
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

[00:00] >> Hello, beautiful humans. Welcome to another episode of Teach Gen Tech
[00:06] with one of our favorite returning guests, Ben. >> Hello, I'm back.
[00:12] I wanted to prove to myself and to the world that I could talk about
[00:16] something other than accessibility. Instead, I'm talking about
[00:20] a semi-obscure static site generator today. >> That is also accessible.
[00:26] >> Yes, yeah. >> We're getting there. We are getting there.
[00:34] >> I can come out of my shell a bit. >> I am very, very excited for this one
[00:42] because we've had a few people on from Netlify, and I'm very excited that I'm finally learning Netlify.
[00:50] But then on last week, Nick from Netlify came on and was talking
[00:57] about using Eleventy and I was like, I get it, but I don't get it.
[01:04] How you go from A to Z, and then you offered and I was like,
[01:10] "Yay, this is going to be great." >> I want to ask you before we go in,
[01:18] what have you heard of Eleventy? In your mind, what is it?
[01:21] Or is this like a completely blank canvas? >> I think it's easier to show you.
[01:29] Give me a second and get a browser. I need to present my screen.
[01:47] There we go. I can do this. Is your website SomeAntics or is it BenDMyers?
[01:57] >> I've got two websites. One is BenMyers.Dev,
[02:00] the other is SomeAntics.Dev. They're both Eleventy.
[02:04] >> When I think about Eleventy, I don't know, it's the layout.
[02:12] But this is part of it that I don't know if it's something that your site does because of Eleventy,
[02:18] or if it's something else. But it does this.
[02:21] >> I added the highlights myself. Actually, all the design here is mine,
[02:27] which I think is going to get us to a very interesting point about Eleventy,
[02:31] which is that basically, a recurring theme that we will see today is
[02:40] that Eleventy's only opinion is that it should not get in the way of your opinions.
[02:49] So anytime you're seeing an Eleventy site, it is basically entirely made from scratch.
[02:56] People have gone in and written the HTML themselves, they've done the design work.
[03:00] This isn't Eleventy doing design magic or anything like this. Eleventy is just a tool that some folks have
[03:09] used to create websites with their vision. >> The reason I brought up Nick's website is
[03:18] because it's also the line. The line makes me think Eleventy.
[03:23] >> Because I think that that's just a coincidence, honestly. It's just a coincidence. It's just CSS as Anthony says.
[03:30] We just happen to have similar design interests. >> That is what I know of Eleventy.
[03:37] >> Sure. Eleventy is what's called a static site generator, and Anthony has a great call out in the chat.
[03:44] Have you heard of static site generators, and what do you think those are?
[03:48] >> I'm working on figuring out a word for it. >> Sure.
[03:58] >> I think static site generators are like website builders. >> Sure.
[04:15] >> In the fact that you put content there and it stays there, and a static site generator just helps you generate it.
[04:23] It helps you create it and just put in content. You take content, you put it in there,
[04:28] and you don't have to figure out anything. >> Yeah. A key point.
[04:33] Yeah, you're taking this content, but the output is plain old HTML.
[04:39] >> Okay. >> You've got different web frameworks that
[04:43] all work via different approaches. Actually, maybe I'll just give the world's
[04:49] briefest and most abstract history of web development here. >> I dig it.
[04:55] >> I think that this will actually help. In the earliest days of the web, we want HTML.
[05:03] This is what we've got. That's the language of the web, is HTML.
[05:07] If you have a website, what you've done is you've manually artisanally handwritten
[05:13] some HTML files and you've stuck them on a server somewhere. >> MySpace.
[05:18] >> MySpace comes later. In the earliest days, it is pure static.
[05:28] You've written some HTML and it lives on a server. It's unchanging. It only changes
[05:36] when you go in and manually update those files. It's very artisanal, very handcrafted.
[05:41] We run into some problems because handcrafting files like that, you don't get dynamic contents.
[05:48] You can't respond to things in real-time and you can't really accept user submissions and stuff like that.
[05:55] You want websites that can change over time. Think about, for instance, what if we built a lovely website or whatever,
[06:03] and then where we created every HTML file individually. Then later, our business partners come back to us and they're like,
[06:10] "Jen, we need to change the nav bar." You have to go to each of those HTML files and manually edit the nav bar.
[06:18] That's painful. You don't want to do that. Different approaches spin off of this problem.
[06:26] You want to be able to change things across a lot of pages at once, and you, in many cases,
[06:32] want to respond to real-time changes to data. One approach you can have is called server-side rendering.
[06:39] This is where you've still got a server, but anytime someone's device reaches out to that server,
[06:45] that server builds a new HTML page on demand. This is in the early days,
[06:52] this is using tools like PHP or Ruby on Rails or ASP.NET. A lot of those tools are still in use today.
[07:02] But that's the general idea. As you reach out to a server,
[07:05] that server creates a new page for you. This is pretty cool because that server can keep track of who you are.
[07:12] This is what's called a session. It can update things in real-time based on who you are.
[07:16] It's customizing a page for you. But servers have their own downsides.
[07:22] One, maintaining a server, painful. You don't want to do that. No one wants to maintain a server.
[07:27] Also, if your website goes viral and gets way more traffic than you expected,
[07:32] the server goes down. No fun. These are some trade-offs you get from there.
[07:37] Hey, we got lots of fun folks in the chat. Howdy, howdy. >> I'm trying not to giggle as you're talking.
[07:49] >> So good. There's other approaches. You end up in this world called client-side rendering,
[07:56] which is where frameworks like React will basically ship a ton of JavaScript.
[08:00] So you ship a mostly minimal HTML page that links out to a giant JavaScript file that the user also downloads,
[08:10] and the JavaScript goes through and creates all the elements of the page. This gives you immense flexibility, which is incredible.
[08:19] But it comes at the cost of things like web performance, because it turns out, broadly speaking,
[08:25] doing things with JavaScript is slower than doing things with just raw HTML. There's other things too.
[08:32] >> That's where things like QUIC or NUX3 work with hydration. >> Yeah. Basically, folks start hybridizing these approaches.
[08:44] What if we could have something that created raw HTML, but then also linked the JavaScript necessary to make this into
[08:52] a dynamic interactive experience and stuff like that. But all this while, the dream of just having
[09:00] HTML files on a server like pre-made HTML files, that dream never died.
[09:06] Some people decided to write quick scripts that could take your content and just apply some HTML around it,
[09:14] and then generate some files, some boring HTML files,
[09:18] and you could stick those HTML files on a server or a content delivery network of your choice.
[09:23] That is a static site generator. It takes your content,
[09:28] smacks it into some HTML, and then at the end of the day,
[09:32] you've got some boring HTML files. The biggest static site generator historically has been Jekyll,
[09:41] which was built in Rails. Sorry, built in Ruby. That's the correct wording.
[09:45] But my favorite static site generator is Eleventy, which takes a lot of inspiration from Jekyll,
[09:53] but it's built in JavaScript. It's built for Node.
[09:57] That's what we're going to be doing today, is we're going to be playing with a script where
[10:01] it'll just transform content into HTML. We decide what that HTML looks like.
[10:06] We decide what the styles are. All it's doing is handling the piping,
[10:11] the content into the HTML that we specify. >> To Anthony's comment really quick is Jekyll was created by
[10:19] Tom, the same dude that created Redwood in GitHub. I was like, "Tom, MySpace?"
[10:25] >> No, regrettably. >> I'm very stuck on MySpace apparently right now.
[10:30] So really quick to add to what you were, and just fact-checking myself, I guess,
[10:37] is when I was comparing Squarespace, Squarespace isn't because it's mostly in, let's see,
[10:48] I'm seeing CSS, so not necessarily HTML? >> It's hard to tell with this view.
[10:59] I'm not actually sure how Squarespace handles this. >> Okay. I'll Google it another time.
[11:05] >> Yeah, so Eleventy, all you need to know really is that it is a factory that
[11:13] takes your content and just transforms into HTML, and it's incredibly flexible.
[11:19] We're just only going to scratch the surface of it today. What I want to build is a pet showcase site.
[11:26] This is inspired by my friend Mike Aparicio, who has his own pet showcase site also built with Eleventy.
[11:32] It's Dogs of Dev. So if you go to dogsof.dev,
[11:36] you'll see today's inspiration. We're not going to make anything as pretty as this,
[11:41] but this is the inspiration. You can click any one of these dogs and it'll
[11:45] take you to an info page about those dogs. >> But they're all so cute.
[11:50] >> They are. >> I don't know which one to click.
[11:53] Okay, let's click this one, Nova. >> Nova. We can see that Nova is owned by Robert Perez,
[11:59] who is a senior full-stack engineer. This one has a bit of a description.
[12:07] This tells you a bit about Matilda. >> And lives out.
[12:11] >> Yeah. We're not going to have anything quite as complete as this.
[12:15] But Dan Mall is an incredible figure in the field of design systems.
[12:24] So good. Okay, cool. So we're not going to get
[12:32] anything that looks quite as good as Dogs of Dev. It's not going to be quite as complete,
[12:36] but that is the general idea, is we're just going to create a pet showcase project.
[12:40] Cool with you? >> Cool.
[12:42] >> Awesome. >> Yes.
[12:43] >> So ahead of time, I created a repo that just has
[12:46] the bare minimum boilerplate and not even that. Mainly, I just didn't want to have to struggle
[12:52] through installing everything ahead of time. We just took care of that.
[12:58] But yeah, so we've got an incredibly small project. Actually, do you want to link out to the repo so that
[13:04] folks at home can see what we've already got? >> Yes, already did.
[13:09] >> Cool. >> We're talking. For anybody curious,
[13:14] all the work that Laura and I did on Monday, I can't open code dot.
[13:20] It's still too much work today. So I'll be troubleshooting that later.
[13:24] It's going to be great. >> All right.
[13:27] >> But yes, this is the repo. >> Yeah. So let's go ahead.
[13:36] I mean, maybe we just create our own first bit of content.
[13:41] So go ahead and open up that source directory. Inside source, there's already an assets folder,
[13:47] but can you add just, here we go. Yeah, we got a few pets.
[13:52] We've got my tuna and cupcake, and we've got your Kiona.
[13:57] >> She likes to get made into the bed. >> Nice. So can you just go ahead and inside source,
[14:05] create a new file, let's call it like test.md.
[14:10] I noticed that VS Code is nesting this, so it's put test.md inside source/assets.
[14:19] Can you just click and drag that to the word source? There you go. Cool.
[14:25] So how's your markdown? Are you good with markdown?
[14:29] Are you comfortable with markdown? >> Comfortable, yes.
[14:32] But I do always look at the cheat codes, so that way I'm like, "Okay, cool."
[14:39] >> Sure. Let's just put in a bit of markdown, not too much, just a little bit.
[14:45] Let's put a first-level heading, so you're just going to do a pound sign.
[14:49] Let's do a quick space, and then just add just a little bit of text.
[14:58] We're eventually going to remove this file, but this is just to briefly show us what Eleventy is doing.
[15:07] Go ahead and hit "Enter" twice, and then maybe put in a quick sentence of text or something like that.
[15:20] Maybe surround the word "better" in asterisks, so we can get some italics going on.
[15:47] All right. Let's go ahead and save this and open up our terminal. You'll want to save the file first.
[15:58] >> Oh, yeah. >> Yeah.
[16:00] >> You did say that. >> All right. We're going to run a command,
[16:04] and this is going to be npx space Eleventy. This is going to run Eleventy on our file,
[16:13] and it's going to just make a build of our site. We're going to see a few things here.
[16:20] Now, in your directory, you've actually got a new folder.
[16:25] It's grayed out, but it's called _site. You can pop this open in VS Code if you want.
[16:31] There's an _site directory. It's at the very top of the list.
[16:36] >> Oh, thank you. >> There you go. This is our built site.
[16:42] Interesting. What do you notice? >> It has a README and the source files,
[16:48] so we can put the sources in the source files folder. >> Sure. What it's doing,
[16:56] what Eleventy has done is Eleventy recognizes certain file types as what we call templates.
[17:02] Template is just a file that content can be in. There's several accepted file types.
[17:09] HTML files can count as templates. Markdown files can.
[17:13] Liquid and Nunchucks, which are templating languages, those files get picked up as templates.
[17:17] Eleventy is going to look for every possible template file in the root of your directory,
[17:23] and it's going to go ahead and build it as HTML. If you pop open, for instance,
[17:28] that source folder inside _site, and there's actually this test folder,
[17:36] and inside test, there's index.html. Let's go ahead and take a look at that.
[17:40] [OVERLAPPING] >> Oh, that's fun.
[17:45] >> Yeah, it just created HTML. Now, this HTML,
[17:50] I should say, is not particularly complete. A full HTML document would have a lot more stuff going on.
[17:55] It would have a head tag, it would have a body tag. This is a fragment of
[18:00] the HTML that we would actually hope to have on our page. But Eleventy has taken our markdown and created some HTML.
[18:11] Incidentally, it's done it again with readme.md, which is just this project level thing.
[18:17] So if you pop open readme and pop open index.html, you can see it's done the same thing.
[18:25] >> That's fancy. >> It is. Now, Eleventy,
[18:36] by default, is going to use our top level directory. But if you think about it, that's not especially helpful for us,
[18:46] because in a lot of real-world projects, we like to use the markdown files in the top level,
[18:51] or just any file in the top level really, for project metafiles in a way,
[18:57] things like readme or contributing. We don't want that to live on our website.
[19:02] So let's go ahead and configure Eleventy. First, let's go ahead and delete the underscore site directory.
[19:09] This way, we'll get a completely fresh build. We won't have leftover artifacts.
[19:15] You'll notice that there's this file called .eleventy.js. This is an Eleventy config file.
[19:25] I have added in some comments that are going to help us do some autocomplete. Those comments that you see there are completely optional,
[19:31] but it's just going to help us with some autocomplete that we've got. You'll notice that it's returning this object on line 7.
[19:40] >> Yes. >> Go ahead and inside that object,
[19:43] just go ahead and start a new line. We're going to configure Eleventy's input directory.
[19:49] We're going to tell it, "Hey, even though the root of the project is this, we actually want source to be treated as the top of our project.
[19:56] That way, everything is relative to source. Things that are outside of source don't get wrapped up in our site."
[20:02] The way we do that is we write dir, short for directory, so that's D-I-R,
[20:08] and then backspace one, and then hit colon. This is going to be an object,
[20:15] so hit space, and then you're going to do some curly braces, and hit Enter. Now, we're going to specify input.
[20:24] Start typing input, yep, colon. This is going to be a string,
[20:31] and you're going to put SRC for source. You're going to save this. Now, let's go back to
[20:41] our terminal and let's just rerun that npx eleventy command. Let's take a look at our new underscore site.
[20:55] What do you notice? >> It only has the.html, index.html.
[21:04] >> You'll notice it's inside test. If this were deployed on a site,
[21:08] a user could go to your URL slash test slash, because basic default browser behavior,
[21:17] if there's an index.html inside of a directory, then you don't actually need to say index.html.
[21:24] This has created the slash test slash route. It's a little harder to tell because, again,
[21:32] VS Code is combining nested folders, but you've created a slash test page.
[21:39] >> Got it. >> Cool. How are you feeling about this so far?
[21:44] Things making sense? >> Yes. It's giving me ideas of where to continue researching so far,
[21:52] but at the same time visualizing it actually as it shows up too. >> Yeah. Tell you what,
[22:01] can you pop open that package.json file? That's package lock. You want the one that's right in front of the package.json.
[22:12] Notice on lines 6-9, we described some scripts.
[22:17] There's a build script, which maps to eleventy,
[22:21] and there's a dev script that maps to eleventy dash dash serve. From now on, we're not going to run npx eleventy.
[22:28] If we want to make a build, we can just say npm run build.
[22:33] Or even better, for local development, we might want a dev server that responds to changes as we make them,
[22:40] that we can go ahead and pull up in our browser. That's going to be dev. In your terminal,
[22:45] can you run npm run dev for me? >> Is it run dev one word or two words?
[22:52] >> Two words. There you go. It tells you that this is hosted at HTTP colon slash slash localhost 3000.
[23:04] Let's go ahead and pop that up in our browser. >> Also, as a heads up,
[23:11] JBW, it will also be available on YouTube right away. >> Yeah.
[23:21] >> It doesn't always like to do things long. >> Nice. Let's take a look at this.
[23:28] This is actually going to error out because we don't have a root page. There's nothing at slash,
[23:36] but there is something at slash test. Go ahead and update your URL to the slash test.
[23:44] There you go. We're going to have two windows on screen at the same time. One will be your browser smooshed to one side,
[23:55] and then the other will be your terminal. Sorry, not your terminal, your editor.
[24:00] >> Hey, this is my camera that I use. It's cool that it does random things.
[24:07] >> Yeah. I want to show you, you'll probably have gotten similar experiences like
[24:15] this from other frameworks you've used. But as we make changes,
[24:20] now that we're running the dev server, as we make changes,
[24:22] our site will update automatically. Let's go back to that test.md folder.
[24:28] I filed it. There we go. Yeah. Go ahead and just make a small change.
[24:33] Yeah. Go ahead and save, and boom. It's already updated on the left-hand side.
[24:50] >> Oh, that's fun. >> Yeah. Prior to Eleventy 2.0,
[24:57] actually Eleventy actually technically is not on 2.0. We're using a canary release of 2.0.
[25:02] But prior to 2.0, Eleventy used a dev server called Browser Sync.
[25:08] But now Eleventy has its own custom dev server that adds a lot of niceties like this.
[25:14] It removes some of the pain points that we will never have to see in our learning process.
[25:20] Just to call out, this is Eleventy's own custom, homegrown dev server, and it is incredible.
[25:27] Cool. But we're not here to just see some words on pages. We want to see pets.
[25:33] That would be cool. It would be nice to have some pets.
[25:37] Let's go ahead and I think every pet should have their own page. What do you think?
[25:45] >> Yes. >> Okay. Now I'm going to ask for your opinion.
[25:50] When you visit this on your website, should those pages be like slash cupcake,
[25:56] or should they be something like slash pets slash cupcake? >> I would say slash pets slash cupcake because if I want
[26:06] to be able to add more to the site. >> Yeah, it's a good strategy.
[26:11] Inside source, create a pets directory. >> Anthony answered their own question.
[26:24] That looks like no, but Vite is, Vite is an option.
[26:31] Is it using Vite under the hood or not? >> All right. Yeah, and inside pets,
[26:37] let's go ahead and create a markdown file called Kiona.md. Don't know why the cursor didn't land in there.
[26:47] Sometimes that happens with VS Code, it's weird. >> All right. Let's just do some really rudimentary things with this.
[26:57] Let's have an h1, so that's just one pound sign space and then Kiona.
[27:03] What are some details you'd like to have about Kiona on this page? >> All right. We can't just use h3s for everything.
[27:22] That's not accessible, friend. >> I know. I was just thinking about that and then I was
[27:26] thinking that I can't do after the line, so I'm going to have to do bold.
[27:32] Can you do bold? I don't remember. You can do bold. >> You can do bold. Bold can be double asterisks around things.
[27:39] >> Okay. Yeah, that's what I was thinking. >> You could also alternatively do double undersource.
[27:46] There we go. >> That's what I was thinking to do,
[27:50] but it wasn't like. What up, Bakari?
[27:53] >> Hey, Bakari. >> Then we'll do.
[27:59] >> We want to breed. All right. Nice, nice. >> We got a question in the chat about when will 11d 2.0 be released?
[28:29] There's no date yet, but if you look at 11d's 2.0 milestone on GitHub,
[28:37] you can see that it's getting pretty close. Zach seems pretty confident that it's nearing completion.
[28:43] No known date yet. Then tell you what. Let's have
[28:53] one more detail here and let's have that be the owner name. >> I'm cheating y'all,
[29:12] because in the other side, I'm like, I know I can do this.
[29:16] How do I go look up to do the HTML? >> Cool. In your editor,
[29:29] can you go ahead and just, oh, sorry. Yes. Let's go ahead and finish.
[29:36] >> Is it this? >> Are you trying to do a link?
[29:44] >> Yeah. >> It's square braces for the link text
[29:46] and then followed by parentheses for the URL. >> Okay. I had it backwards.
[29:52] >> Yeah. For reasons, let's maybe, we can have this be a link for now.
[30:01] I think at some point we might roll back the link bit, but let's go ahead and yeah.
[30:08] Then maybe go down a few lines and let's just add a sentence about who Kiona is or what her personality is like.
[30:19] >> Nice. All right. >> Let's go ahead and save this and then in your browser,
[30:51] we can go ahead and see this page already. It will already be at, well, yeah.
[30:58] Brilliant. >> This is fun.
[31:04] >> Yeah. It's nice to see how quickly you can get things up and running with this.
[31:13] >> All right. >> Do you want to include a picture of Kiona now?
[31:32] >> Yes. >> We have these pictures already.
[31:36] There's this source/assets folder. But if you were to open up under source site,
[31:42] which again is the finished product, it's the built site,
[31:46] you'll notice that assets are nowhere to be found. Our images aren't there.
[31:50] This is because Eleventy by default only cares about templates basically. That's the only thing that's going to make it through.
[31:59] If you want stuff to end up in your site, you have to tell Eleventy specifically to do that.
[32:04] The way we do that is by opening up.eleventy.js, which is our Eleventy config file.
[32:10] Inside that function, but before the return statement, so between lines 6 and 7.
[32:15] Yeah. Go ahead and type Eleventy config. Yep.addPassThroughCopy.
[32:27] There you go, that one. This is a function, so go ahead and do some parentheses.
[32:38] Then I think, yeah, so let's go ahead and start a string.
[32:43] In here, I think we can just say source/assets. You've got an extra S before the T that you're going to want to
[32:56] remove because the word assets is surprisingly hard. Let's go ahead and save this and see if this works.
[33:10] We can totally do that, Anthony. I just wanted to see if this works.
[33:16] Can you pop open underscore site, and we'll just see if assets was copied over.
[33:22] Not quite yet, doesn't seem to have done it. What if you removed source,
[33:28] like the source/ part? We'll see if that does it.
[33:36] I think the problem then is, if you revert the source/,
[33:41] I think we actually have to restart our dev server because we've made a change to the core configuration here.
[33:47] >> Wrong clicky clicky. >> You're going to do Control C, and that, yep.
[33:58] We'll see if this has done it. Interesting, still hasn't.
[34:07] >> Would it be the weird squid? Is it the squiggly thing, this thing?
[34:11] >> I don't think you need to do that. Let me check on one of my projects real quick.
[34:17] Let's try, here's how I've done it. It's actually dot slash source/assets.
[34:31] Dot and then slash, and then SRC, you've got SCR.
[34:38] >> That could also be it, y'all. >> Yep. This should work.
[34:44] We can save this and we'll restart our dev server. Goodness. Why? What is this doing?
[34:59] This is identical to how I have it on my site. Interesting.
[35:07] >> I'm very prone to doing this. This is like what happens on Teach Gen Tech.
[35:14] >> Let me try once more on a different site, just to confirm.
[35:25] But what this is supposed to do is just straight up, do nothing to the files.
[35:29] It just takes the directory and just copies it over. Can I ask you to just once more try this,
[35:43] but /assets/, because it's a directory. Sorry, /source/assets/.
[35:57] We'll see if this does it. Restart our dev server.
[36:04] If this doesn't work, we'll pivot away from. We are going to pivot away from this then.
[36:13] Go ahead and comment out that line. Unfortunately, no images for now.
[36:17] We will have to fix that in a return episode. Go ahead and comment out that pass-through copy line.
[36:27] Cool. >> No. Sorry.
[36:32] I'm trying to remember what Laura taught me, so give me one second.
[36:35] It was like whatever mark thing that you're in, it will. >> Oh, command slash.
[36:46] >> There we go. I was doing the different direction.
[36:54] >> I got you. We'll go ahead and save this. You don't need to restart anything.
[36:59] Unfortunately, images, it seems like, will not be cooperating for us today.
[37:08] >> Yeah, there's the side conversation happening about an HTML element that you could have used to represent
[37:19] those details about Kiona. But I've just decided to keep things as simple as possible,
[37:32] so we're just not going to introduce that right now. >> Let's go ahead and go back to your Kiona markdown file.
[37:41] Seems like this is unsaved, so go ahead and save it. Cool.
[37:52] The next thing that we're going to want to do is. >> It said one was unsaved, so now it's unsaved.
[38:02] >> The next thing that we would want to do is if you look back at the Kiona page in your browser,
[38:12] you'll notice that as we talked about before, this is bare bones.
[38:17] It added no extra HTML. You have to add the HTML.
[38:21] You have to tell it what it is that you want it to do. Let's go ahead and do that.
[38:28] Let's add some HTML. What we're going to do is we're going to add what's called a layout.
[38:32] We've got our template, that's the markdown file. Basically, Eleventy is going to drop the built contents of that template,
[38:41] the built HTML, into a larger HTML context that we get to specify. We'll see what that looks like.
[38:50] >> If you wanted CSS, would you put that in here too?
[38:54] >> You could. I've got thoughts about how we could do CSS. But yeah, you would want to handle that at the layout level.
[39:03] >> Then you might be answering this already. Does that mean we could use Bedrock in here?
[39:11] >> You could use Bedrock if you wanted, yeah. >> Okay.
[39:14] >> But I would have to look that up more specifically. But for now, let's just see if we can get the HTML wrapper around this.
[39:22] If you right-click on source in your File Explorer, and we're just going to create a new folder,
[39:32] and this is going to have a very specific name, which is underscore includes.
[39:42] This is a magic name that Eleventy knows about. You have to call it this.
[39:48] Or there's an explicit configuration you can supply to rename it to whatever you want.
[39:54] I don't see the point in reconfiguring that. I like to keep things with the defaults as much as possible.
[39:59] In here, we can create our first layout. Let's go ahead and create inside your underscore includes,
[40:05] go ahead and create pet.html. This will be the HTML that gets applied to every pet page is our thought.
[40:13] In here, go ahead and hit exclamation mark and hit "Enter". VS Code has an extension called Emmet that supplies some handy shortcuts.
[40:26] This way, we've got the base HTML page that we want. Let's go down to line 10,
[40:36] and let's go ahead and create a main element. Let's go ahead and actually above the main element.
[40:55] Between lines 9 and 10, let's go ahead and add a header element.
[40:59] Not heading, but header, yeah. Cool. In here, go ahead and put an anchor tag,
[41:08] so a, we'll have the href will just be slash. This will point to the homepage and go inside the anchor tag,
[41:18] and we'll give this a name of pets of teach-gen-tech. Let's save this.
[41:30] Now, we want to apply this layout that we've got to our content. We want our Kiona page to use the pet layout.
[41:43] Go back to kiona.md. At the very top of this document,
[41:48] we're going to do something called front matter. The way you do that is you do hyphen, hyphen, hyphen.
[41:54] >> What's a hyphen? I don't know why. >> Dash, dash, dash.
[42:02] >> Okay. >> Sorry, that's a slash.
[42:04] You want like a minus. We want three minuses.
[42:09] Go ahead and on the next line, do the same thing, three minuses.
[42:15] Then in between those, we're now using a syntax called YAML,
[42:22] which some folks might be familiar with already. It's like an alternative to JSON.
[42:26] We're going to put the word layout. Again, this is a magic word.
[42:30] It has to be this for Eleventy to pick this up. Now, we're going to do colon, space.
[42:36] Go ahead and do pet.html. What this says is that Eleventy is going to look inside
[42:43] your includes directory for a pet.html file. It's going to go ahead and apply it.
[42:49] As you can see over on the left-hand side, it's applied it. If you were to inspect element
[42:54] and take a look at the DOM that was created, it would exactly match your pet.html file.
[42:59] There's just one problem. Can you name what that problem might be? >> Yeah. It's not showing everything else in the file.
[43:08] >> Great. Yeah. Eleventy doesn't know where to put your contents. We have to tell it. Go back to
[43:16] your pet.html layout and inside main, we're going to use what's called some templating syntax.
[43:22] This is basically some syntax that Eleventy is going to process and inject some stuff of our choosing.
[43:29] Go ahead and hit "Tab" for me. You're going to do double curly braces.
[43:36] Here we've got magic name, content, and save.
[43:44] >> Yay. >> Boom.
[43:48] >> Okay. >> Kind of fun.
[43:51] >> I dig it. >> All right. Maybe now we add some other pets. What do you think?
[43:58] >> Yes. We would add a new. >> Yeah. Let's go ahead and start adding another pet.
[44:06] Right-click on pets and let's add cupcake.md. Because we've already got some stuff for a dog,
[44:17] we can copy a lot of that stuff over, right? >> Then we can.
[44:23] >> All right. Cupcake is a multi-poo.
[44:43] Her birthday is, God, I want to say it would be October 15th, 2010, I think.
[44:59] She's also 12. You can go ahead and replace this with Ben Myers, benmyers.dev. For a brief description,
[45:17] let's go ahead and put enemy to stuffed pigs. Let's save. You can now go to the cupcake page.
[45:33] >> All right. >> If we were able to get the images to work,
[45:50] it would be in the Eleventy.js. What would we add?
[45:57] If we got this part working, what would we add to here to show the photo?
[46:03] >> You could do, so the markdown syntax for an image is exclamation mark.
[46:08] Then in square brackets, you would supply the alt text for the image.
[46:14] >> Alt text. >> Yeah. Then after that,
[46:19] you put parentheses. It looks a lot like a link just with
[46:23] a exclamation mark at the beginning, and then this would be the image source.
[46:27] >> Which I'm going to comment this out. No, damn it. I did it again. It's this one.
[46:39] Because if I did it, it would be alt text.
[46:50] No, wrong one. Alt text. >> Then for image source,
[46:57] that means it would be forward slash source. >> It would actually, source
[47:03] doesn't exist in the final project that gets built, so it'd be assets/cupcake.jpeg.
[47:11] >> I don't think this will work, and I know that you have to go soon,
[47:17] so that's why I was like, if I could work on that. >> But we haven't gotten to some of my favorite parts of Eleventy,
[47:24] so I want to spend some time doing that, which is this notion of data in Eleventy.
[47:30] Because if you think about it, what we've just done here is some very manual duplication.
[47:37] If the site gets big, and we had a lot of contributors, for instance,
[47:43] this page, updating all of these pages, if we decided we needed to rearrange on all of these pages,
[47:53] we wanted to put owner right under name or whatever, we'd have to go back and update this for all the pages,
[47:58] which runs us into that same problem we had with the artisanally handcrafted HTML pages with that one.
[48:06] It said, for a lot of these things that are common between pages, we want to shift as much of these things to the data and to the layouts.
[48:14] I want to show you something. In your front matter, and let's go ahead and do this for Kiyona,
[48:18] because we love Kiyona, Kiyona is special. In your front matter,
[48:23] so that's the bit between the minuses, we can just add any property we want.
[48:30] Let's put name, our dog name or pet name rather, or something. I would recommend doing this all lowercase or doing camel case rather,
[48:40] so lowercase p, capital N. We'll put Kiyona. Yeah, you format this as you would.
[48:53] Similarly, we could put breed. >> Okay.
[49:00] >> Lowercase b probably. >> That's going to take me a sec to get used to, but yes.
[49:06] >> Sure. >> Okay.
[49:07] >> Old dog mix. >> I can do just those two for now.
[49:13] >> Yeah, let's do that. Then fun fact, or I guess fun little tidbit, on line 8,
[49:20] replace the word Kiyona with double curly braces and put name. Sorry, pet name, pet name, yeah.
[49:34] On line 9, replace old dog mix with double curly's breed. On the left-hand side, just to confirm that this works,
[49:49] let's go back to the Kiyona page. Yeah, in the browser.
[49:56] What we've done basically is we've added extra metadata around this page, and then we've used that metadata.
[50:03] But things get even better. In your pet.html layout,
[50:10] we can use that same data that we just created. Under main, so between lines 13 and 14,
[50:19] go ahead and add an h1 element, and then do some double curly's and pet name.
[50:30] It just added that. Now, let's go back to the cupcake markdown file.
[50:44] Let's start bringing some of those things back in, like doing the same thing.
[50:48] In your front matter, yeah. Pet name, cupcake, breed Maltipoo.
[51:04] >> I was just saying cupcake. >> Yeah. We can actually remove
[51:26] the pound sign cupcake headings from both cupcake.md and kiyona.md. There we go.
[51:42] Now, our heading is controlled by our layout, and whoever's writing the markdown file
[51:46] doesn't have to remember to add the heading. They just need to add the necessary data.
[51:51] Go back to your pet.html layout real quick. Hey, there. Did I lose you?
[52:04] Again, you there? I can't. Okay. For Jen's John, interesting.
[52:34] Sounds like we need a part two then. Semantic takeover. Yeah, this was the plan.
[52:53] Just completely takeover, kick Jen out, make her lose internet.
[53:03] Goodness. Well, in that case, I have to figure out if I can even end this stream.
[53:08] I should be able to, but I don't know if I can.
[53:14] Interesting. Jen, I don't think I can stop your stream. I can't share my screen either.
[53:24] I don't have that privilege though, Anthony, because I'm not actually like a mod of this stream.
[53:34] Oh, wait. Hang on. Incredible. All right.
[53:42] Jen. Well, that's fun. I'm probably going to go ahead and just leave
[53:54] the studio then and here's hoping the stream goes well from here on out or just keeps going until Jen can log back in.
[54:05] Because I have to get to a meeting, but we will do a part two.
[54:08] Part two will happen. Bye, y'all. [MUSIC]
[54:16] [MUSIC] [MUSIC]
[54:36] [MUSIC] [MUSIC]
[54:56] [MUSIC] [MUSIC]
[55:16] [MUSIC] [MUSIC]
[55:36] [MUSIC] [MUSIC]
[55:56] [MUSIC] [MUSIC]
[56:16] [MUSIC] 
