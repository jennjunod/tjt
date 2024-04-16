---
showLink: "https://www.youtube.com/watch?v=sAl1EwqlSgo"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-native-web-components-with-chris-ferdinandi-gomakethings"
title: "Teach Jenn Native Web Components with Chris Ferdinandi @gomakethings"
publishDate: "2023-05-19"
coverImage: "https://i.ytimg.com/vi/sAl1EwqlSgo/maxresdefault.jpg"
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

[00:00] another episode of Teach Gen Tech and today we are here with Chris who has definitely helped rattle in some of my ADHD-ness of like actually posting stuff. So thank you for that and thank
[00:15] you for the reminders and you know getting things moved along. But Chris what are you going to be teaching us today? Hey everyone, so today we're going to be talking about browser native web
[00:27] components. What they are, what they do, how they work, and when and why you might want to use them. Yeah so should be fun. Yay and tell us a bit about yourself. Yeah so I'm thank you for having me by
[00:42] the way. I am a wow I can't talk about who I am right now. I teach yeah the ADHD is kicking in hard right now. I'm sorry. I teach people JavaScript. My whole thing is that I believe
[00:59] there's a simpler and easier way to do a lot of the things that we do and I think a lot of modern best practices are both bad for the web and make things harder for us as developers. So I kind
[01:10] of spend a lot of my time pushing back against that. And yeah as part of that I have a daily newsletter that goes out to about 14,000 people and I'd love to have all you wonderful viewers on
[01:24] it. Yeah so throughout what we're talking about today I have put together a ton of related resources and a link to the source code over at gomakethings.com/teachgentech. So if you want to
[01:42] head over there and grab that and follow along you're more than welcome to or after the show if that's easier. But I just want to make things as easy as possible for folks.
[01:50] Yay and yes as a recap because I know in the show we do things a little differently every time of like hey are we going to be talking theory are we actually going to be talking about like coding
[02:06] itself coding proper and before I go into what we're actually doing I do want to say thank you Ben Myers for joining. You're one of my favorite people too. It's kind of crazy how Ben, A) Ben
[02:25] hasn't been on the show for forever we do need to change that Ben. I don't know like life happens which is weird because I feel like I talked to Ben really recently but if I look at our like
[02:33] like our chat then it's been like months that I'm always like how did this happen? I don't okay okay yet Ben has also introduced me to Josh Goldberg who has been doing our TypeScript
[02:50] series which has been super super fun. I enjoy learning about TypeScript. It's also been fun because I don't know the ins and outs of JavaScript. So learning TypeScript and JavaScript
[03:02] I almost feel like it makes TypeScript easier because I don't know the differences but it makes trying to like know what to fix a bit harder and yes so today I'm going to be
[03:17] taking notes while Chris talks about what we'll be doing today. You know I'll do it on my handy dandy iPad like I've done before and taking notes and then if we need to swap back and forth I will
[03:30] but for the most part Chris will be sharing his screen and then we'll bounce back and if you have questions please make sure to drop them in the chat because we will go over them and you know
[03:42] ask as we go and yes. Please I was gonna say I really interrupt as much as you want if anything I'm saying either doesn't make sense or you want to dig into anything please feel free to
[03:56] interrupt me. Cool will do and are you ready to get started? I am yeah. Okay I will add your share screen to the screen but also everyone I did link the gomakethings.com/teachgentech
[04:15] so that way you can follow along and also you can find how to find Chris at the very very bottom and make sure you go follow Chris on all the things. I'm really impressed that you know the
[04:33] difference between a forward and backslash because I always get them wrong or confused I can never I can never remember. Oh did I say it? You did yeah you said forward slash.
[04:44] I think it's because I used to work in I worked for GoDaddy which is all about domains so we would have to say it all the time but if I were looking at it in a in a code editor
[04:56] I wouldn't know which one's which but because I I'm so used to saying domains I know how to say it but that's that's a great call out. This reminds me of when you used to
[05:08] have to say the www like you ever watch old commercials yes yes where they read out the whole thing http colon slash slash. Yes I agree I agree but we have a roll six and a roll d6 and a roll d20.
[05:28] We do yeah so we're gonna be a little nerdy today. I'm excited. Ben and I played D&D together so Ben knows I'm a big RPG fan and yeah so today we are we're going to build a web component that people
[05:48] can use to roll digital dice on a website or a web app. We're going to start by taking a traditional javascript library that does the same thing and we're going to slowly convert it over
[06:00] into a native web component and we're going to talk along the way we're going to talk about some of the benefits some of the downsides and challenges and weird gutches that you might run
[06:09] into and hopefully explore when you might want to do this and when it's not necessarily the best choice. I like the references you went to because I was playing D&D. I did my first tabletop game as
[06:26] D&D and we just went over to playing The Expanse which is a d6 not the d20 and so I'm just excited that I actually get to understand what you're saying but then also a different Chris was on
[06:44] last week and I asked we were short a player so I asked Ben and I asked that Chris I was like y'all we're short a player on The Expanse. Ben was spoken for so I reached out to Chris and Chris
[06:56] was like yo my wife like loves The Expanse and I'm like yay! How does the game compare to the show? Is it good? Because I love the show. I've torn through all the books. So far we're only on
[07:09] episode one and I may not be the best person to ask because this is all new to me. The Expanse is new. Oh you're I'm so jealous. Yeah it took me years to read the book series and now I feel
[07:21] hollow and empty inside so. Oh gosh oh gosh. Well you get attached to your characters and then it's all over and you're like what do I do now? This is so true. This is so true. Okay so we've got
[07:32] our dice. Yay we got dice. I'm very excited about our dice. All right you get some dice you click them it tells you what you rolled. Relatively straightforward. So the example I have here is
[07:45] like a traditional JavaScript library. So if we jump over to the text editor I have a button with like a class on it for styling and a unique id so we know what it is and I've got my role of d6 text
[07:59] and then I've got an ARIA live region that we render the results of the role into and as an ARIA live region if someone's using a screen reader it will announce that role to the screen
[08:12] reader so that you know visually impaired folks know what the hell's going on. What that is so cool. So with this one we're using it's just to start it's a maybe a more traditional JavaScript
[08:29] library so I've got I've got a JavaScript class. I'm not going to go into all of the specifics of it just yet because we'll get into that as we start converting this over into a web component
[08:39] but the way this works is you can create a new dice object by using the new keyword and the constructor object so new roll dice and then you pass in a selector string for the dice and the
[08:57] element to render it into and you can optionally pass in an object of options if you want to customize anything so if I wanted to change the size of the dice from its default of d6 I can
[09:09] pass that in as a size property. If I want to change the display text that shows for the result I can pass that in as a string and this has this handlebars-esque little thing that gets replaced
[09:19] out so with the d20 it says result instead of you rolled a yeah so pretty basic library here and then you know you can style things with with CSS so I've got I've got my my styles up here just
[09:34] to control the the different dice and that's why they have these like slightly different colors and appearances. So this is typically how JavaScript libraries work and it works pretty well but
[09:47] it has some potential I don't want to say potential issues but there are some some things with it that especially with like larger components can be problematic.
[10:00] So really quick for example oh sorry quick you might be going into this with the example but yeah sure also for some reason me and classes yeah just don't click. Yeah I heard you talk
[10:16] about that actually in your React episode a few months back. Yeah yeah I also talked about it I don't think I did it on stream but y'all learning TypeScript with Josh Goldberg it is such a dope
[10:30] human and fun but what we were looking on is we just finished chapter six and chapter eight is what I fear most classes I'm not looking forward to it it's not exactly what he said
[10:49] if I wanted to I could skip it it's not going to be the end of the world but I asked that because it's still something that doesn't click as much so by any means you're using classes is that going
[11:01] to be a requirement to these web components? Yes and we will we will unpack that as we go so I'll make sure that we don't we can ignore it for purposes of this like traditional library but
[11:17] we can absolutely unpack that as we dig in actually you know what Jen no we're going to talk about this right now hold on just a second ready okay no time like the present so are you
[11:32] are you a little bit more comfortable with like prototypal inheritance and using like object prototypes is that kind of how you typically work or do you not do that either? I typically go
[11:42] hey I want to build this I have no idea what it's actually called or how to do it so but I figure out enough to get it to work. Sure so here let's do a really dumb example okay okay I'm excited so
[11:57] let's say I have a library called greeting okay and I want to be able to do something like let's say let josh equals new greeting I don't know what josh is always my go-to name I don't
[12:12] know why so we want to be able to do something like like this right so we're gonna say josh say hi and that should like I don't know log hi josh into the console or alert it somewhere do
[12:24] something like that and then I also want to be able to say bye this is like the dumbest simplest example so this is what this looks like in a like a traditional object oriented
[12:35] programming kind of setup I've got my constructor function here which I've called greeting and when you create a new greeting you pass in like some sort of variable in this case a name and I'm
[12:48] saving it as a property of the current item which is what this is so each instance will have its own name property and it's whatever you passed in and then I can attach functions to the constructor
[13:02] prototype so in this case we have say hi equals function and then we're also going to do one for say bye and because these are attached to the prototype they get access to this and any
[13:17] properties that are associated with it so when I run this function I could do something like hello we're gonna go this name right and then you know we're gonna say you know hey name gtfo right
[13:38] so let's actually just pop this over into a browser so we can we can see it here boom so you can see now we've got hello josh and hey josh get the [ __ ] out and you know you could do this
[13:49] with like a different name right so I could have toby equals new greeting this reminds me I really want to re-watch the office right so well toby say bye hey toby gtfo if I do josh again you know
[14:03] it's it's still going to say josh because this information is tied to each each unique instance um okay so the the prototype is letting you access all of the properties of that instance
[14:16] classes make writing these a little bit simpler and they also add uh in newer browsers like just a buttload of new new features that make things really nice um so you can have um uh private um
[14:34] private properties and functions that are only accessible inside inside the class and can't be read or accessed externally um and all sorts of really fun stuff that I won't get into right now
[14:46] but if I were going to rewrite this as a class I write class greeting and this becomes an object so instead of having to define you know function greeting and attach things to the prototype
[14:57] I just write class greeting and then um uh the constructor is always named constructor but it otherwise works exactly the same way so here we're gonna we're gonna say name we're gonna say
[15:10] this name um and then for my say hi and say five say bye functions um I just write them like this I shouldn't say just just as like the worst word in uh in teaching code but uh I can go like this
[15:28] and um these automatically get attached to the instance prototype um and so what's nice about this is you create this little scoped object like normally if I wanted to scope this stuff
[15:41] I might have to like wrap it in an immediately invoked function expression or put it in an es module or something I just I get I get everything kind of contained in this one little object
[15:51] um and this does exactly the same thing as this they're just two different ways of writing it um it's maybe a little bit more nuanced than that there are a couple of like
[16:03] weird little gutches and things um like for example with traditional object-oriented programming you can do this without the new constructor or instantiator
[16:14] and it'll still work with classes you're forced to use new which is good um but uh yeah that's classes in a nutshell and hopefully as we start to dig into this a little bit more it will make
[16:26] more sense and if at any point you feel like it's not making sense Jen let me know and we can dig into it thank you for that and I will say like what you're saying makes sense as a I would you
[16:42] say that in and this is going off of like the first linkedin learning that I ever tried was javascript and I've got I've been stuck on the way I've learned it tried learning it from
[16:53] there but do you need classes to be in a different file or they normally in a different file no they don't have to be um you can drop everything in one one file if you want um a lot of folks
[17:09] put them in different files and import things because that's kind of the the modern way people do things but um okay uh for our purposes I'm literally just everything
[17:20] is in one spot like I have a single html file for each example and uh that's how we're getting down so so for on this one if I'm doing like the constructor or that version as a class if I
[17:33] had it in a different file I would just do export uh so it knew what to export yeah so let's say this was either one of these in their own kind of file somewhere I'm just going to add some white
[17:45] space so it looks like it's on its own um I could go export default greeting or if you prefer to not have a default you could do that um okay and then in another file I can import I import
[18:00] okay this function plus all of the prototypal functions that go with it uh all of its instance methods there we go that's the official name would come along with it um I think you just
[18:11] answered the question like the way you described classes made sense to me it was like that added to not understanding import exports when I very first started I think out of the extra complication okay
[18:28] thank you thank you for the side track no no worries that's I'm all about tangents it's a superpower so um so circling back uh one of the challenges with traditional um uh
[18:44] components and libraries is um all the html right so um I have I have all this html here and if I'm kind of handing this along to a developer to use I'm trusting them to not fuck
[19:03] it up um so uh in particular one thing that could easily get dropped out is if someone forgets to add aria live to the um the container that the dice roll result is going into now visually impaired
[19:19] people are people who rely on screen readers not going to be able to know what those results are they won't get any sort of information from this um uh this library it matters a little bit less
[19:31] but like a lot of times you'll have libraries where you also load a style sheet and it's got a bunch of styles that control how things look and behave um and uh if I type a class wrong
[19:45] on one of these elements those styles won't get applied maybe I already have a thing in my library or in my my app or my site rather that has classes with the same name and now they're in
[19:57] collision with each other um and so uh web components aim to solve a lot of those issues um so let's take a look at what a web component version of this might look like so you can see
[20:11] what I'm talking about um so here um instead of having all of this stuff I have a single custom element here roll dice and we're going to build this up so that it replicates all of the stuff
[20:29] that was in our uh traditional library and so right off the bat the ergonomics for a developer who's doing this become a lot easier uh all they have to do is make sure the javascript that powers
[20:43] this is loaded and drop this element somewhere on the page and all of the other stuff like all of the kind of the other things that go into here will get automatically added for them so they don't
[20:56] have to do anything there um uh we're also going to as we move further into this look at how we can scope um or um uh I'm forgetting the word and it starts with a c um uh keep the uh keep the
[21:15] classes and elements inside here from um colluding with other uh um other elements on the page that have the same name um basically by putting everything in its own little dom called the
[21:28] shadow dom um so we'll take a look at how all this works as we carry on uh but for now I just want to show you if I open up this page um the styling isn't here right now but I have my little roller
[21:40] d6 button clicking it does nothing I haven't added any functionality I just want to show you the basics of how we go from this to having an actual button here and if I inspect really quick yeah uh
[21:56] I don't know why it took me so long to have this click but I'm very excited so astro components are web components right I would think so you're good so um um not exactly
[22:14] um well maybe I've never seen a live output from astro before I've seen how stuff goes in I know the big kind of the one of the big things with astro is what you type in is getting compiled
[22:29] into something else so I don't know if the output is actually web components or not but we can find out pretty easily uh let's see astro they have a new new website now so let's see um it's possible
[22:45] they're not building their own site with with astro so so um it's tough to say but these do not look like web components to me um but that doesn't mean maybe someone in the comments will
[22:58] know because I haven't played with astro uh all that much thank you and and the reason I was bringing up astro is because it's when I first used components um and uh ben answered I'm just
[23:15] trying to finish this thought and then we'll uh reply with ben um read ben's reply there we go um of what it's like I remember you showing how uh in the code that it was showing the dice the roll
[23:32] dice and having that just there I was like oh that's like an astro component and that's kind of what made me put two and two together um let me read all of ben's uh replies of astro components
[23:49] are basically compiled into the underlying markup it's different scenario than custom elements like this actually being added to the dom astro does actually use web components to handle some of
[24:02] its lazy loading functionality but your components are not themselves really web components thanks ben really quick remind me what is dom like I feel like I should know that but I don't
[24:16] know why object model um so it is the interface that javascript and believe it or not some other programming languages like python use to interact with html elements so I've got a button element
[24:31] and then the dom or document object model is the interface that allows various javascript methods to interact with that element um and it's all weird and heady and confusing so that's about
[24:46] as much as I know about um you know just that's perfect that is perfect thank you so so you'll notice here though what we entered into the page is this this empty element but what we have kind
[24:59] of rendered out is paragraph with the button and my aria live element on the page so let's take a look at how we actually do that um so uh with um web components you are going to create a class
[25:17] that extends the html element object um and uh I'll get into kind of the nitty-gritty of that in a minute but once you have created a class to do that um you can then define a custom element
[25:36] um I like to this is probably not as necessary now uh in a world of modern evergreen browsers but here I'm just checking that the custom elements property actually exists as a thing you can run
[25:46] and as long as it does I'm going to use the custom elements define method I pass in the name of the custom element and the class that I want to use to control and
[25:58] power it um one little note about custom elements with native web components they have to include a dash uh so I couldn't just call this dice it's one of the like the guardrails that um
[26:13] allows you to create custom elements knowing comfortably that they will not collide with existing real elements um that are just kind of standard in the browser uh so custom elements
[26:26] always have a dash in them and uh regular regular standard elements uh do not um and that way that the the twain never never shall meet um so within a custom uh web component class um you have a
[26:47] couple of things the first is the constructor uh and this is the thing that um uh this will run automatically uh when when the browser loads and the javascript for the web component runs
[27:01] and you know as long as you've defined that custom element if the browser detects the custom element it's automatically going to instantiate a a version of it for each element on the page and
[27:15] inside this constructor the first thing you need to do is run the super constructor and that gives you access to all of the properties that are part of this html element class that roll dice is
[27:27] extending or that your custom web component is extending and then i'm not using shadow dom yet but i am rendering some html into the page so when this is instantiated i am using the inner html
[27:42] property on this which in this case is the element itself uh to inject some content into it and that's how we end up with our um our markup in the ui even though we didn't actually physically type
[27:57] it um there is a life cycle for web components so they're instantiated and then um they get connected in the dom which is when they actually kind of get like appended into the ui and when
[28:11] that happens this connected callback function automatically runs if at any point the element is removed from the dom uh say if i used like the remove method or i moved it i maybe i grabbed the
[28:23] element and i used like the append or prepend method to move it around the page somewhere this disconnected callback method would fire and if it was getting then re-added somewhere else the
[28:33] connected callback would run again um so if you for some reason need to kind of fire things off when stuff gets injected or removed from the dom you have some hooks to do that um really quick
[28:44] yeah um does super need uh the with rounded brackets need the uh need parameters no no you just you just run it um uh i'm actually let's see what happens if i don't yeah so um now i'm getting
[29:04] this must call super constructor in derived class before accessing this and so it's really it's what gives you access to the this keyword so all i have to do is run it uh i know sometimes you see it in
[29:13] examples with arguments uh for this particular use case we don't um here you can see connected is actually logging into the console gen and that's happening right here so when the element
[29:24] gets uh appended into the dom um and i could even do something like so uh let's say here i'm gonna cheat i'm gonna use the uh that dollar sign shorthand that's built right into into browsers
[29:37] because i'm feeling lazy so here i've got my my roll dice element um and if i were to remove it like that now that disconnected callback function runs because i disconnected it from the the
[29:52] document object model or dom um but so this is this is kind of the the basics of it here so um if you had an element that had no interactivity to it you just wanted to render some piece of ui that
[30:08] had a bunch of pieces to it into the dom and uh that was it you were done with it but you wanted to make it easier um say like a like a nav menu that just had some links um and you wanted to
[30:19] just be able to do like um you know like main nav or something like that you could do it like this um i don't think that really warrants a web component but you theoretically could
[30:29] could do it and then you're all set um obviously that's not necessarily a great great use of this technology um but it probably could serve a purpose in something like a design system
[30:43] where um you're really trying to ensure a specific look uh and consistent kind of layout or way of doing things across the system um but we're going to make this more interesting
[30:56] by adding interactivity because that's where these things really shine um so let me pull up my next example uh so um here what i want to do is actually make it so that when you click this
[31:12] button something happens so um the first thing i am going to do is after i instantiate my constructor i'm going to assign a dice property to it and this is going to be an array of dice
[31:28] values in this case one through six because we're just going to go with a standard d6 for now and inside my connected callback i am going to set up a click event listener so that when
[31:42] my button is clicked i roll the dice quote unquote and display that value into the ui so um in this particular case i need to get the button uh rather than requiring the user to pass
[32:01] in specific selectors and things we can use query selector inside our parent element that roll dice custom element by using this so in in the context of a custom element or a web component this is
[32:15] going to refer to like the the custom element itself so i'm saying inside my roll dice element i'm going to use query selector to find the button that i injected up here if there isn't one for
[32:29] some reason there should be but if there isn't um we'll just we'll quit early with the return operator but otherwise we're going to add a click event listener to the button uh and then whenever
[32:41] that fires we are going to look for the aria live region inside um inside that parent element one little one little thing here uh you'll notice i'm using host um which i have i have assigned
[32:55] this to so once you move inside this callback function uh this no longer refers to the parent element it refers to something else i forget what i think it might be the function might be the
[33:07] window um so i just i cached this to host up here so that i can use it inside here i think i could have avoided this with arrow functions but i hate them so uh here we are um so i'm getting the aria
[33:21] live region and then um i'll explain this in a second but i am i am shuffling my array so i'm just randomly sorting it and then i'm grabbing the first number from the now scrambled array
[33:33] and displaying that as the result using the text content property um if we jump over to the browser you can see it actually works which is cool um so this shuffle method this is where
[33:44] we get into classes and your your hate of them gen so please feel free to dig into this as much as you'd like um so uh i have shuffle as a static method that means it's attached to roll dice
[33:59] instead of the specific instance um jumping back over actually this might make more sense here right so uh let's say we had greeting um shout right as a function so um in this case uh we're
[34:16] just gonna say hey you right so because this is not attached to the prototype um i would not be able to do josh shout that wouldn't work because it's not attached to the prototype which ties it
[34:32] to specific instances instead i would have to run greeting shout and i always have to call it on that main object uh in javascript classes static methods work the same way so i'm now assigning
[34:47] this hash shuffle method to roll dice instead of to my specific custom element or instance and then the reason i'm using the hash before it is that makes it a private uh function that can only be
[35:02] accessed inside the class which means you can't call it anywhere else and there's no real reason to do that here other than just like uh i don't know not wanting people to potentially overwrite
[35:15] it or mess with it in any way um so it's just a private method it's only used inside this function and or inside this class and that's it um and this is using something called a
[35:25] newt yates i think is the name of fishery yates there we go or newt is the other name for it but it's a it's a because javascript does not have a native array shuffling algorithm this is a really
[35:37] good way to shuffle an array that produces more random results than just using math random wood i'm not good with algorithms i i copy pasted this off the internet but
[35:48] fair enough yeah so it's shuffling the array and then taking whatever the first number is and injecting into the ui and that's basically the whole thing on this one we've now added a
[36:01] little bit of interactivity and all the user had to do was load the javascript file and put the element on the page they don't have to create a new um you know like a new instance of it or
[36:12] instantiate anything it just you know you just load the file and load the element and it does its thing um so right off the bat we've got some wins with our web component here um there may be
[36:26] instances where you want to remove interactivity so let's say for example i remove this button off the page i remove the element um eventually the browser will garbage collect that event
[36:40] listener but if we don't want to wait for that to happen um uh or there's other things that might not get garbage collected um we can remove that interactivity um as part of our disconnected
[36:53] callback um so uh in this particular case in order to do that we need to have access to the uh excuse me the handler function um that was used to create the event listener in the first place
[37:10] so i want to be able to use the remove event listener function and i need the exact same handler that went in so um we are going to create another static method called create handler that
[37:25] we're going to use to make that event listener function um so i copy and pasted the stuff that was in there and i just moved it to this create handler method that returns the callback function
[37:36] and then when the constructor runs i'm creating my handler and assigning it to a this handler property so that we can access it in our various methods um before i move forward does that make
[37:48] sense because i know classes are kind of like uh oh my god i don't know what's going on for you i just want to make sure that actually makes sense so where i'm at right now i would
[37:57] say that i'm mostly conceptually getting what you're saying there are a lot of things where i haven't necessarily put together words with though okay um and i'm almost thinking i'm like
[38:10] i want to continue in the fact that i'm like okay like this is soaking in this is more of like theory explaining it and then maybe i or you and i i vote for the latter but can come on and actually build
[38:22] it from scratch because it's like now that i understand the overview and are like getting there i'm like i can actually learn it with implementation because i've realized like when
[38:33] you're looking at it on the code itself i'm like oh i'm pretty sure i've done that but i had no idea that what a handler is or a super construct but i'm like i'm pretty sure i've done those but it's
[38:46] not yeah like this is something that i've been struggling a lot with is i don't necessarily have the words to go with what i've done and so therefore it can be hard to follow along the
[39:01] burden of being a self-taught developer um yes because i i feel you there it's taking i've been doing this like a decade and it's taken me a long time to be like okay i know what's going on and
[39:10] even then not always yeah so like i'm i'm like i'm enjoying this um and i i'm like okay so i mean what you went through with the classes is helping me stay like being able to stay where you're at
[39:26] and i'm writing down the words that i'm getting stuck with so that way it's not super distracting us but like enough that i'm like okay i can go look these up
[39:35] offline to when i review this again okay that sounds great um yeah so just for anybody who's like i don't know what's going on here um uh i'm passing the instance in to my create handler
[39:49] function i'm assigning it to this host variable uh and then that that gets me around that whole like this keyword scope to the function kind of thing um so i'm doing the same exact stuff i was
[40:00] doing in my event listener callback function before um i'm returning that callback function out and i'm just saving it as a property on on our instance and you'll see why in just a second
[40:13] so now inside my connected callback function when i run my button add event listener method instead of passing that anonymous function in straight up i'm passing in this handler which
[40:25] is now a reference to that function that we created and the reason i do that is so that when i go to disconnect it later and i run my button remove event listener method i can pass
[40:38] that same handler in in order for this event uh the remove event listener method to work it needs to be run with the same exact arguments as the ones that were used to create it in the first
[40:50] place so that means it needs to be run on the same element and it needs to have the same callback function passed in um uh so we get around that by doing what we just did here so if i were to open
[41:03] this up um uh everything continues to work uh as expected and then if i were to um here we go let's do this roll dice remove so if i were to remove that from the ui um uh as part of that process
[41:22] the event listener also gets cleaned up or removed um just real quick by the way i'm just i want to make sure everybody knows this is not jquery um uh don't use this in production but browsers for
[41:33] like debugging purposes uh have a shorthand uh so the dollar sign and then any valid css selector will get you the first matching element and uh if you use two dollar signs it will return an array
[41:47] of all matching elements so if you're too lazy to type out document query selector or document query selector all like i am um this is a really great way to just do some quick debugging in the
[41:58] console thank you for that call out you're welcome uh it's one of my favorite debugging tricks so um cool so now we're going to get into why the shadow dom matters so uh and what it even is
[42:14] actually uh so you know right now we're just we're injecting our content for this custom element directly into the regular dom um the plain old uh ui and um that can lead to some unintended
[42:31] side effects so for example uh here i have um i have set pointer events on buttons to none and aria live has a display value of none uh this is stupid for two reasons one i can't click the
[42:46] button at all um but so let's go ahead and we'll comment that out so that i can uh now when i click the button nothing is um is being rendered into into the ui um oh actually we got we got multiple
[43:00] issues happening here so hold on let's let's get rid of that for a sec here we go so what you can see is i'm actually having a result get displayed in the ui um but because i have this element set
[43:15] to hidden it's not showing up uh it's just visually not there i'm another really dumb thing that a user could do is get that element and remove the aria live attribute off it entirely
[43:27] if they wanted to um uh and so uh if you did that like let's say i was no longer display none in that um uh here we go um oh yeah now now the result isn't even rendering
[43:42] because the attribute that you need to render it isn't there um uh but assuming it used some sort of other selector you could have a situation where the text shows up but it doesn't get announced to
[43:54] visually impaired users um and so uh the idea here is that you want to be able to encapsulate content inside this custom element to prevent it from being messed with in other parts of the code
[44:11] um because it's very unlikely that someone would do this kind of thing maliciously it's a lot more likely that someone has some piece of styling or javascript functionality where the selectors they
[44:22] use have an overlap with the same selectors you've used in your component uh and then you run into these weird unintended side effects um especially as you have larger projects with bigger teams and
[44:36] maybe you have multiple teams working on different pieces of the same app it's increasingly likely that you'll have components that have the same class names on them even though they're totally
[44:44] separate and do totally different things um and so the shadow dom is a feature of web components that aims to fix that so here let's close out some of these many many tabs that i now have open um
[44:59] so you can see here again i'm still in this this file i am still saying pointer events none re live display none um but i am doing something a little bit different inside my constructor
[45:14] so after running my super constructor i am creating a shadow dom inside my web component so i'm saying this root so i'm assigning a root property inside my web component and i'm running
[45:30] the attach shadow method now this has two methods opened and closed if it's open you can use javascript to pierce into it and manipulate some of the elements the default value or default mode
[45:45] closed blocks javascript from getting in but css is always blocked from piercing through so many global styles you have will not affect the content inside and then when i go to render oh sorry go
[45:59] ahead jen yeah that's good to know and ben asked a question of um because they had to step away for a moment of did we talk about display none and how that removes uh the live region from the screen
[46:14] reader output and i know that we when you were doing the screen reader or when we were looking at it it didn't have anything in the divs is that like we're were we talking about it there where
[46:28] it changed it to display none or did i just miss that part no there's a couple things that happen so with css where i've got this display none um situation going on here it both uh removes it
[46:43] visually from the ui and then because it's not being displayed it's also not being um announced so uh there are changes happening but nobody can see them and screen reader users don't get those
[46:54] announcements either um the other boneheaded thing i was doing was removing the aria live attribute entirely so um uh even if text was being rendered in and could be seen it wouldn't get
[47:08] announced um got it and these are just like weirdly specific examples like it could be one of a million different things it could be even just like something as simple as like oh this
[47:17] this element is a weird color the text is off because it shares a class name with some other part of the ui that you didn't didn't realize and so shadow dom is an attempt to prevent a lot of
[47:28] that um and so instead of injecting my html directly into the element i now inject it into this dot root which is where we've kind of assigned our newly created shadow dom and so if i
[47:44] were to open this up in the browser um and inspect this element uh you can see i've got the same content here but instead of being directly underneath my roll dice element it's now in this
[47:59] shadow root uh element here or object um and uh you will sometimes notice this with um browser native web components as well um that add additional stuff um i'm trying to think of one
[48:16] off the top of my head i want to say details and summary do this with some of their elements but i could be wrong there um uh but what i've done here is i've created these elements that now exist
[48:28] inside their own dom and so when i push my uh my roll button here this content continues to show up no don't open don't open slack what are you doing here um uh even though i've got no pointer events
[48:45] set on my buttons and aria live has display none none of that is affecting these elements because they're encapsulated in their own completely separate dom away from my main dom where all
[48:57] this other stuff lives um if i were to say try and remove aria live from that element um i'm actually going to get an error in the browser uh cannot read properties of null uh i literally
[49:11] can't even get this aria live element because it's hidden inside the shadow dom and i have that set to closed um just so you can see the difference here if i were to set that to open um uh oh no
[49:25] what's going on maybe i'm wrong about that or i'm typing it wrong also possible um either way can't mess with it um so it keeps it i'm gonna have to figure out why that is later uh protected
[49:40] isn't live uh demos always so fun because you never know i'm like i it's very possible i either type something wrong or have something wrong in my head um so that gets us into some other cool
[49:55] features that we can take advantage of now that we are inside the shadow dom uh and one of those is slots so you may recall from our original uh our original kind of setup here we had some
[50:08] interesting icons going on um and uh we even had some different text and right now user has no option for that because we are just or the developer has no option for that because we're
[50:20] just rendering this fixed button into the ui so as you can see from this ui we now have some different different things showing up let's take a look at how we actually make that happen
[50:33] so uh i've got one that is just my standard roll dice element and then i have a few others that have these spans in there with this slot attribute on it and some associated name so i've got one for
[50:48] icon i've got another slot for text and i've got one rolled eyes element that has both and slots provide your web component with a way to have default content that will show up and also let
[51:06] developers who use your thing hook into them and customize them with their own information instead so i find that things are always a little bit easier with an example so let's take a look
[51:18] so uh inside my inner html here now i am using slots for i'm just gonna change the layout a little bit so this is easier to see so inside my button i now have two slot elements and each one
[51:31] has a name that matches the the slot properties that we used up top you know so we've got slot icon slot text these don't have to be spans they could be anything could be like a div or
[51:44] whatever you want but since everything's in line here i'm just using spans um and so what this is saying is i have a slot with a name of icon and this is the default that i'm going to use for it
[51:55] i'm going to use this dice roll emoji and i have a slot with the name of text and that default text is roll a d6 if someone does not include an element with a slot property whose value match
[52:08] or slot attribute i'm sorry whose value matches this name it will use this default value if they do provide one it will use that value instead uh so you know now i can do things like say okay i
[52:22] want the icon to be this bearded wizard dude and i want this text to be toss some cubes so in this case it's going to say roll d6 but it's going to have the wizard here it's still going to use the
[52:34] the dice emoji but it's going to say toss some cubes instead and in this one i'm customizing both and if we jump over to the browser you can see that's exactly what we get we get that default
[52:44] text with the different emoji default emoji with some different text and everything customized slots are totally optional but they provide these really nice hooks that you can use
[52:55] for developers to customize the stuff that's being spit out while still providing a baseline default experience if if you want one um and also not giving them too much you know it gets back to
[53:10] um you know if we were doing this the traditional way where the user has to write out all the html they could already do this but they could also miss things like the aria live attribute and so
[53:21] this allows some customization without giving them control over stuff that they could break or get wrong if that makes sense okay it does okay you have questions i do but i don't at the same time
[53:38] it's like i kind of have to noodle on it because something that is like coming to mind and it was something i asked about earlier is more of just like um going between like dom and shadow dom
[53:54] and then uh the nesting of things and i'm like i feel like that is going to be something that it takes time not necessarily something to like super dig into i will say something that
[54:13] if you could go into this a bit more of sure throughout the entire um going through everything you talked about being able to i believe it was connect and disconnect and i'm like but why would
[54:29] you want to connect and disconnect when you just wanted to like do its own thing and it should auto disconnect yeah so these callback functions the connected callback and the disconnected callback
[54:40] you're not running those directly these are callback functions that fire automatically when the element itself uh so in this case roll dice if it gets added to the dom or removed from
[54:57] the dom so uh you theoretically want to do things if i were to take this element and remove it from the ui you might want to run some code in response and in this case we're just attaching and removing
[55:08] event listeners but um you know it could be something like calling an api endpoint or running some other piece of code to like show up in its place or something like that um it just
[55:21] provides a way for you to hook into okay this element got rendered into the dom or this element got removed from the ui um and you don't have to use them at all um generally as a recommended best
[55:36] practice that's where you want to add or remove your event listeners um because you don't need them until the element is in the ui um and once it's removed from the ui you don't um but you
[55:48] could not use them at all i've seen web components where all of that stuff just happens in the constructor and you don't use these callbacks at all um they just provide a you know kind of a
[56:01] a way to extend your component um and you're never going to run them directly um they are they are things that run in response to um dom interaction because these elements are um elements in the page
[56:14] so you can use other javascript met like and dom manipulation methods to move them around and do stuff like that okay why would especially when we're talking about like the button being removed
[56:31] and then needing to disconnect the callback for the event listener that's totally making sense but at least knowing me and just trying to get stuff to like work and not work yeah i i tend
[56:44] to do the comment out situation where you comment something out see if what happens and then uncommented out is like how how would someone know which way to go or is there just like a
[57:02] best practice there to to like instead of like commentating out to turn off the event listener or something like that something that you may suggest to just get used to this in all in many
[57:15] situations or yeah um so i one thing i guess i will just kind of make note of is this thing where i'm like removing the event listener it's optional like eventually the browser is going to garbage
[57:32] collect that um i'd be like oh this element isn't here anymore we don't need this anymore gone um so you could just as easily take all this stuff and drop it up here like if you're just getting
[57:46] started you just drop it all in the constructor and never worry about it again that's totally fine too um in fact my first few web components that's how i wrote them i was clean and simple
[57:57] and easy um i'm making this a little bit more robust just because i want to be able to cover all of kind of the different different things you can do with a web component but that doesn't mean
[58:08] you need to do all of them okay um so very cool very cool uh one other thing you can do speaking of kind of interactions because we were just talking about how this is like a you know it's
[58:21] an element in the dom so um one thing you can do with web components is detect when attributes have been added or changed in value on the element and um respond to it in some way so for example uh
[58:39] let's say we wanted to provide a way for like this being used in a tabletop rpg um app right and you want developers to be able to turn off rolling of that dice in certain situations like maybe the
[58:56] player is unconscious and they can't roll or something like i don't know whatever it happens yeah right yeah so the way this web component is going to work is a developer can toss the
[59:07] disabled attribute on there and the dice will no longer be able to roll um and you know obviously you might be doing this with javascript so you might do something like um i'm going to get
[59:18] that element with the query selector method and i'm going to use the set attribute method to add disabled and in this case a little value here you can't roll right now so web components allow you
[59:30] to detect that this has been added or changed in value and do something about it and the way they do that is with the attribute changed callback so handful of they're all they all end with callback
[59:43] but there's a handful of methods built into web components that um run when things happen and this one runs when attributes are changed now uh if it ran every time every single attribute on an element
[59:56] changed it could run a whole bunch and that would be bad for performance so in order for this to work um it actually requires you to register the attributes you want to detect so that it doesn't
[60:06] run for all of them uh so in this case we um i don't know why they do it this way but you create a static observed attributes method or static it's a getter method um observed attributes method
[60:21] and it returns an array of the attributes that you want to observe in this case there's just one it's the disabled attribute uh and so um in this particular situation here let's actually
[60:33] comment this out for a second i'm just going to log changed and then it accepts three parameters name the original value and the new value um that's why i'm going to log those things to the
[60:47] console uh and here i'm doing two things i'm setting a hello attribute uh and a disabled attribute and if we jump over to the browser and open up the console the only one that gets logged
[60:59] is disabled because i did not um i did not register the other one as something that should be observed so you can see hello you is on the element but it did not trigger that um attribute
[61:12] changed callback function to run only disabled it um and i get the name of the attribute uh its old value was null because it didn't exist and its new value is you can't roll right now um so let's
[61:26] actually do something with it because there's no real point in kind of uh listening for this if we're not actually going to take action so um in our case let's say when the button gets disabled
[61:38] we want to let the user know um and so to do that we are going to um use the query selector method to get the aria live element inside our shadow dom so in this root instead of just this um and uh
[61:54] we are going to update the this should really be text content not inner html i don't know why i'm doing that let's change that right now uh but so we will update the text content um if the new value
[62:06] has a value of null which is uh what will happen if we remove the attribute it'll have a value of null instead of um uh instead of some sort of string uh so if it's null we're going to wipe
[62:18] that aria live attributes text out entirely um otherwise we're going to set it to the new value and now what ends up happening is i get you can't roll right now so we're letting the user know
[62:32] they can't roll right now um and if i were to remove that attribute so if i say uh remove um what we call this disabled that message goes away um we can also hook into the presence of that
[62:50] attribute uh inside our click event listener so here we're saying if that host element has the disabled attribute on it just return right away don't actually roll the dice or display anything
[63:05] into the dom um so now when i click this element it never updates this because my custom element is disabled and i'm not doing anything um and this is just like an example
[63:18] obviously there's like a million different ways you could you could use this um uh but the idea here is that you can listen for attributes being added or removed to an element um or um uh having
[63:34] their value changed and you can respond to it in some way inside your um uh inside your element it's a little bit like how um for those of you who are familiar with the details and summary elements
[63:46] if you add the open attribute to the details element it will automatically expand and show content so similar kind of thing there you're providing hooks that allow developers to interact
[63:56] with your components through the html instead of directly with javascript um so for anybody here who likes view you might you might enjoy this it's a little bit more like view and a little bit less
[64:06] like react um interesting okay and if i were to remove that disabled attribute uh not only does our aria live region get you know wiped clean but now i can i can start rolling again um
[64:20] and the numbers show up all right well i think i'm pretty good on on questions just because it's it as i said it's a it's a noodley thing you got a noodle on it i although what questions do all of
[64:40] you have because i would love to hear those um i will remove chris's screen just for the moment so we can just focus on the chat and see what everybody else is saying i do want to give
[64:57] a shout out to ben and his show um some antics uh that's just a fun one and uh just tagged it there y'all should also go follow ben uh because ben is who introduced us and introduces me to a really
[65:15] a ton of really dope people and ben is also just an all-around great human oh my gosh i know i i always feel like so weird when i'm like i'm just like people's number one fans and i'm like
[65:28] maybe i'm just creepy i don't know i'm not sure um and then also i'm going to repost because ben also helped uh pin the the actual website that we were working off of and
[65:50] what we'll be going to later on which i'm pretty excited about so let me grab that as well do you think there's anything that we like missed that you wanted to go over that yeah yeah the one thing
[66:07] that i think is probably important to talk about is um so if if the shadow dom blocks css from getting in how the hell do you actually style your web components okay um so if we have a little bit
[66:21] of time i'd love to just yeah kick into a couple of ways to do that but i do want to make sure before we dive into that if anybody has any kind of questions about anything we've talked about so
[66:30] far that we we address that i feel like i i know for some of the streams it's like not a very active stream itself with questions but it's like something people go back through and watch
[66:42] and have questions and i feel like that's also where i'm at because i'm like it makes sense but it doesn't make sense so that means i'm gonna noodle on it and then like next week i'm gonna be
[66:52] like oh damn that totally made sense and now i can go re-watch it and go okay cool let me now ask the questions so let me go ahead and share your screen so you can show that to us oh perfect and let me
[67:06] get out of inception there we go inception mode always so fun oh man um all right cool so styling um uh so there's a few different ways to do this um one of them uh the most kind of straightforward
[67:26] but also i think potentially least palatable is with inline styles inside the shadow dom so here i've created a style element and i've added styles for my button and my button on hover
[67:38] and if i were to open up the page here uh you can see that now my button is styled um and if i were to look inside here i've actually got my little my style element with these styles
[67:52] inside that shadow dom element or shadow root um so styles can't come in those styles don't bleed out into the regular dom they're just they're encapsulated to this to this element um uh so
[68:09] uh yeah so that's cool but um one inline styles kind of suck uh we'll talk about that in a minute uh but the other thing is um this completely strips developers of the ability to actually
[68:28] customize styles um for these things that are going to be rendered into their app so if this is something you know in a design system that's being used by a company you might want that um
[68:39] like you may want to prevent people from tweaking colors and sizes and things but for an open source project that's designed to be used by lots of different people and different types of apps
[68:51] and sites you might want to provide more control so one really easy way to do that is with css variables so while uh css itself doesn't bleed into web components uh css variables or custom
[69:11] properties i think is what they're called there's like an official name for them it's not variables but everybody calls them variables because you define them with with var um those do
[69:22] bleed into uh your web components if you want them to so uh in this example i still have my inline styles but um i am uh referencing css variables as uh their values so here i'm saying
[69:41] if there's a bg color variable use it otherwise use this fallback color uh same thing for border and radius size and text color and all that um and so uh with this type of setup i have
[69:57] some smart defaults i provided developers with some hooks to customize things if they want to and i'm also only allowing them to customize the things i want them to have control over so
[70:08] i would not allow them to say hide this aria live element but there might be a world where i'd let them control the size of it you know so i you know it would be entirely within bounds i think
[70:21] to do something like um you know like font size equals var um uh you know like let's say message size as a property right um and we'll just give it one m by default but someone could control that
[70:36] if they wanted to and so what you end up with is something like this where um you know i've got uh if we scroll up um on my roll dice elements i'm saying i want a default radius of zero not the
[70:50] one m uh that i think i had defined or quarter of an m whatever i had as my normal um if it has a size value of 20 uh we skipped over this but uh you know you can add attributes and properties
[71:04] to things and hook into them when you're when you're creating your um your elements but so in this case for the one that has a size of 20 which makes it a d20 we actually want to go with a
[71:12] different border color and text color and on hover we want the background color to be rebecca purple as well and the color to be white um and that's how you end up with this button right here that
[71:23] looks a little bit different from from that button um uh so that is better um where this approach also kind of falls apart is if you have a bunch of web components as part of a broader system
[71:41] what you're effectively being forced to do is um uh like manually create a bunch of inline styles uh for a bunch of things um and that's and you know there's a lot of like repeating yourself
[71:58] like let's say i have a bunch of different components that have buttons in them i'm now having to define button styles in each of those different components and that really sucks so um
[72:07] one of the ways that uh you can get around this is a newer approach called constructible style sheets and the way this works is you can import a style sheet just like you would import a javascript
[72:24] file so here i've set my type to module instead of just a normal script tag and uh normally you would you would do this like as an external file in an es module but here just because i'm keeping
[72:34] everything in line um i've got it uh i've got it right here um and so i'm importing uh a style sheet from styles.css uh and i have to add this assert type equals css otherwise it'll try and port it
[72:49] as javascript and it'll throw an error um and once i've imported it inside my constructor i can set the adopted style sheets for my shadow dom to an array of style sheets that i want to add
[73:03] and browsers are really smart about this so if i have multiple elements importing the same style sheet it will only download that style sheet once and attach it to the shadow dom for all of those
[73:18] different components so if i were building say a design system for a company this is a really good way to reuse bits of css like button styles and things like that across all of my web components
[73:33] without having to manually inline all my things um because i'm using a es module here i need to load this as a browser i mean as a live server that's not right what am i doing here there we go
[73:53] cool uh and so now again you can see my buttons are styled i have um i have in here this this style sheet uh where i've got that same stuff i was inlining it's now part of this um uh this
[74:08] external style sheet so i'm able to load that up and code some things um one caveat about this so let's pull up firefox for a second i think yeah so this does not work in firefox and it doesn't
[74:20] work in safari it currently only works in chromium browsers and so there's the there's the rub um if you like this type of experience though and you want to use um web components today
[74:35] lit is a tool for compiling them that allows you to use this approach where you create your external style sheets and it will automatically inline them for you um so you
[74:51] do have an option there um uh it is the one thing that kind of falls apart if you want to use them fully natively um and once firefox which supports it behind a flag and safari which doesn't support
[75:05] it at all once those catch up um it will be possible to to run fully native web components and actually kind of style them a lot more effortlessly uh yeah i'll shut up now jen
[75:18] sorry i've been talking a lot do you have any questions anything you want you want to talk about or dig into around the styling piece of it
[75:25] oh hold on i can't hear you and i don't know if it's you or me one sec let me just make sure no it was totally me it was totally me i was on mute that's cool i i do want to say that i've literally
[75:43] done that during conferences when i'm emceeing and then i'm like oh [ __ ] i'm on mute it's really fun to do that in front of like 2 000 people uh so i i think it was a lot i really
[75:56] like that you you also uh referenced it to view and there's like so many different things that we talked about it is something at least for myself i going back to it's so weird to me so
[76:10] the way today feels is like when i was confused about docker because i haven't gone this deep into it yet i am looking forward to reviewing it and unpacking it wait are you not confused
[76:26] about docker anymore because i'm still not as much not as much confused about docker yeah yeah no i i actually get that a bit more but uh but the actual like a lot of what you talked
[76:41] about i'm like these are the i get it but i don't get it and it's a lot of it is practicing it and also as i'm coding myself going okay cool this is something that chris talked about i just didn't
[76:59] know it had a name and that takes time it's like one of the most frustrating parts of learning is i'm like you're a great teacher and what you said does make sense but
[77:11] it doesn't make sense at the same time yeah and to be fair uh in a like a workshop or a classroom type environment this kind of thing would get spread
[77:24] out over like a long period of time and there would be like uh learn a thing go work on it learn another thing go work on it um i threw a lot at you and i'm sorry about that don't be it's i
[77:36] it's one of the reasons i love because i had somebody on the show about it was docker kubernetes and powershell so all very very difficult concepts yet going through it with theory
[77:51] helped me go okay cool i am doing good for a bit and it made more sense and we do have a question uh let's see yeah so we're gonna build a new design system for our company now and even not
[78:09] knowing a lot about web components i think we should give it a shot that so we don't didn't get attached to any specific framework it is it's it's it the moment already web components with lit
[78:24] are production ready yes definitely uh you'd be joining companies like google salesforce github um salesforce is probably the most vocal about it their whole design system is built with web
[78:36] components and they're really proud of it they've talked about it at conferences a whole bunch um github has leaned really heavily into them um uh and uh google uh also has done a lot of work
[78:50] here uh so yeah they're definitely they're definitely production ready oh microsoft too nice awesome thanks ben um yeah i do think uh i do think using a tool like lit is probably
[79:03] where you need to be at for uh you know for kind of production ready i think is probably the right way to describe it as you noted there um one other thing if you need a good starting point
[79:17] um jared white actually just introduced this to me last week uh if you head over to shoelace dot style um it is a web component library um uh even if you don't kind of you might just use it as a
[79:32] starting point or as inspiration um but uh think about it as like bootstrap but with web components instead of uh you know what bootstrap is um all of those were built with lit as well um uh for kind
[79:47] of unifying the css and everything but might be worth a look just if you need some inspiration that's really cool and linked that one as well um anyone else have any questions
[79:59] before we start wrapping up because i know oh uh we got one we got one yay uh what do you think about writing static uh i don't know if i should say pound or hashtag yeah when reading it out loud
[80:16] i know what you're saying yeah so um uh i the reason i have a create handler function that returns another function um is uh ben will help me out ben i this is not the same thing as currying
[80:35] right but it's like a similar kind of concept but the idea is i need a way to encapsulate this and if i had a static variable i no longer have access to the this keyword or the instance
[80:53] which is really important for what we were doing in this particular web component otherwise not a not a bad idea uh just what you know and if i was running a more generic um
[81:08] uh if i were running if i had my component set up differently where i didn't need access to the instance uh that would work well um where like if i only needed the event object for example
[81:25] um in this particular case i did need access to the specific instance which makes what you're describing not viable although there are other ways i could have worked around that like i could
[81:36] have detected the element that was clicked and then crawled up to the parent element and then started doing some stuff that way uh but i think it's a little convoluted uh and i've just found
[81:46] this a little bit more more simple sorry i'm getting super into the weeds not a terrible idea one that um i i think uh creates more problems than it solves in this particular case
[81:58] and again uh and this is the reason why i linked it while you were talking is on uh the site that has all of the notes from today on go make things.com forward slash teach gen tech is down
[82:13] at the bottom is there are ways to get a hold of chris and i say that because yes you can comment on this like it's going to be going to youtube here shortly let us know your questions chris
[82:24] can help reply there it's definitely something that even though it's out of my ballpark right now this is the great thing about this platform is we have access to experts and that is definitely
[82:37] something that i love and thank you for joining us now something we didn't ask in the beginning and i'm curious how did you get into all of this oh that's a whole podcast episode on its own gen
[82:54] yay uh the uh the short version is i used to work in hr i had a blog i wanted to control how it looked more and so i started kind of hacking my way through wordpress i became known
[83:07] as the hr guy who knows web stuff and then one day when my boss and i were trying to like play around with ideas for um like a um like a learning platform kind of thing that was more like youtube
[83:21] and not like sit butts in seats for eight hours uh we couldn't find anybody who could like build a prototype for like less than half a million dollars and so he looked at me and he's like
[83:31] can you build it i know you do web stuff and i was like no i definitely cannot build this and he goes can you learn and i was like i don't know but i'll try and then two weeks later i came
[83:43] back with this really shitty like but kind of functional prototype and that was the moment that i knew i wanted to do this and not hr anymore um i was just hooked and that was that was it for
[83:54] me i love that i love that and i love that you're still doing teaching and and this aspect now and yay well thank you for joining us today chris and i am going to go find someone to raid uh it looks
[84:13] like the only person that i'm following right now is primogen is that how you say his name why am i so bad at saying his name primogen prime prime again prime the dude that's really popular and
[84:28] really funny and does super techie stuff that is where we're gonna go today uh and he does it's very knowledgeable stuff i'm i'm always impressed by it but i'm always it does go over my head but
[84:42] okay y'all enjoy the raid thank you and see you later 
