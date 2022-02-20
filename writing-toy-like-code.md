---
title: "Writing toy-like code for fun and profit"
description: "Thinking about how for a new pattern to be adopted, it needs to gloss over problems and make them trivial to address. Or, for a paradigm shift to be successful, it needs to feel like a toy."
---

Saw this tweet this morning.

<link rel="stylesheet"href="https://tweeet.link/tweeet.css" /><article class="tweeet"><header class="tweeet__header"><a title="View profile"href="https://twitter.com/frontstuff_io"target="_blank"class="tweeet__profile"><span class="tweeet__avi"><img src="https://pbs.twimg.com/profile_images/977873484759158784/mOItIR7M_200x200.jpg" /></span><span href="https://twitter.com/frontstuff_io"target="_blank"class="tweeet__byline"><span class="tweeet__name">Sarah Dayan</span><span class="tweeet__username">@frontstuff_io</span></span></a><a title="Permalink"href="https://twitter.com/frontstuff_io/status/1495217596538531850"target="_blank"class="tweeet__permalink">Feb 20, 2022</a></header><div class="tweeet__body"><span class='tweeet__newline'>Interesting how <a href="https://twitter.com/remix_run">@remix_run</a> is making server-side rendering cool again.</span><span class='tweeet__newline'>JS devs got mocked for "not using servers" but it reveals is how insufficient traditional server-side frameworks have been to create great UIs.</span><span class='tweeet__newline'>It’s not that we hate SSR. But it wasn’t that great until now.</span></div></article>

Gross generalization: it's interesting how we went from server-rendered sites with JS sprinkled in (RIP in peace jQuery, or [maybe not](https://twitter.com/mikesherov/status/1443679254009483273)), to SPAs, and then back to server-rendering with stuff like Next, Nuxt, etc.

Was this entirely motivated by making developer experience (DX) easier?

I.e. demand for advanced frontend interactions precipitated React et al. React precipitated boilerplates and SPA frameworks, which made it easier to work with. SEO requirements and the difficulty of writing isomorphic React applications precipitated Next.js et al. And now that we've realised SSR isn't so bad, we're back to server-rendering and islands architectures in full framework form, like Remix and Sveltekit.

"Islands architecture" isn't new, it what we did before we had all these other options. But it was pretty manual up until now. And maybe that's the real lesson here.

I'm not sure how to phrase it. It's essentially: for a new pattern to be adopted, it needs to gloss over problems and make them trivial to address. For a paradigm shift to be successful, it needs to [feel like a toy.](https://cdixon.org/2010/01/03/the-next-big-thing-will-start-out-looking-like-a-toy)

There is a spectrum of ways to solve the problems that frameworks like Remix solve. It goes from compose-many-libraries-with-disparate-APIs-into-a-cohesive-system → simply-install-Remix. It's obvious which one most people are going to choose.

For library and framework authors, here's another way to put it:

<link rel="stylesheet"href="https://tweeet.link/tweeet.css" /><article class="tweeet"><header class="tweeet__header"><a title="View profile"href="https://twitter.com/ryanflorence"target="_blank"class="tweeet__profile"><span class="tweeet__avi"><img src="https://pbs.twimg.com/profile_images/1344410501309030403/L2rNpO6h_200x200.jpg" /></span><span href="https://twitter.com/ryanflorence"target="_blank"class="tweeet__byline"><span class="tweeet__name">Ryan Florence</span><span class="tweeet__username">@ryanflorence</span></span></a><a title="Permalink"href="https://twitter.com/ryanflorence/status/1494108702986551298"target="_blank"class="tweeet__permalink">Feb 17, 2022</a></header><div class="tweeet__body"><span class='tweeet__newline'>My dad is an audiophile. He loves speakers. He doesn't listen to music, he listens to speakers. The speakers are the product.</span><span class='tweeet__newline'>It seems a lot of developers are like that. The website/app doesn't matter, it's the code and tech they get to use to build it that matters.</span></div></article>

I'm definitely guilty of thinking more about the tech when writing libraries, and less about "will the average person grok this and know what to do with it."

I need to start writing code that's more toy-like if I want people to use it. Good goal for 2022 I suppose.
