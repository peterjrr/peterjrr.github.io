---
title: Design files are disposable artefacts and code is the source of truth
date: 2021-04-19 16:42:00 Z
layout: post
---

I’ll be the first to admit that my design files are a bit of a mess. I’m a design team of one and my files are full of unnamed layers, wonky spacing, copies of copies of frames and explorations that got abandoned midway through a flow. But here’s the thing. That might actually be ok.

Before the web, most visual designers were graphic designers. They designed for print and the physical space. It is a predictable medium with fixed size formats and content that does not change. When a designer outlined a file ready for the print, that _exact_ design would be replicated in print. 

Websites and apps don't exist in such a predictable environment. They exist in code which is a rich, interactive environment. Screens change and adapt dynamically based on content, language, screen sizes, devices. A single screen could have an almost infinite number of combinations.

### The real source of truth
The people who use our apps and websites never see our design files. I’m afraid, that no matter how hard we try, our beloved pictures of websites and apps are not the source of truth. The only thing that actually matters is the code that gets shipped to production — because that is what our users will see and experience. 

So where does this leave us? Should designers code, or should designers do something else? 

### Communicating design intent
Instead of viewing our design files as the absolute source of truth and trying to replicate every possible state of every screen, a better way to think about our design files is as artefacts that we use to communicate our design intent. With each iteration of a design we are trying to communicate *just enough* to move the needle in production. 

Sometimes you will need a detailed and redlined design file. Sometimes all you need is a sketch on a napkin, or to sit down and have a chat with an engineer and collaborate in code. Remember hovering art directors?

### Redrawing pictures of code components
But if a designer wants to start with what already exists in code, they must redraw a picture of it in order to use or iterate on that thing. 

This is completely bonkers because code components contain so much rich coded behaviour like interactive states, responsive resizing, and designers have to manually recreate all of that. On top of that we have to label and annotate components and add links to the documentation for the actual code component. 

### Designing with code components
At [Interplay](http://interplayapp.com) we’ve been busy working to enable designers to get closer to the real thing and handover more useful artefacts for developers (yes, handover is a dirty word, but until designers can contribute directly to production code there will still be a handover. And yes, we’re working on it 😉.). We built a Figma plugin which replaces your design library in Figma and makes all of your production code components and tokens available directly in Figma. 

Aside from never needing to maintain a design library in Figma again, the magic with this approach is that the rendered Figma components maintain a 1:1 connection with the code components. 

What does that mean? It means that you can design with the latest components, exactly as they are in production. 

It means you get a visual properties panel of all the React props, so designers can fully understand the capablities of the component and have a truly shared language with engineers — when an engineer talks about a prop, the designer isn't saying, "What's a prop?". 

It means that when you live preview your design from Figma, you can run the full React code in the browser. 

It means that when engineers inspect your design file they can copy out JSX of the exact component config (not a link to a docs site or a Storybook file). 

### Deeper thinking about higher level problems
So, of course our design files do actually matter. Our files need to be adequtely tidy and well organised to communicate our design intention. But they aren’t the the end goal in themselves and it’s time to stop treating our design files as the ultimate source of truth.

When designers no longer have to spend their time producing detailed, but disposable, design artefacts for handover — every state of every screen with redlines and annotations for spacing, sizes and colours — our headspace is freed up to think about higher level things and ultimately have more design impact.

If this way of working resonates with you, [drop me a message](mailto:pete@interplayapp.com) and I’d love to show you what we’re building.