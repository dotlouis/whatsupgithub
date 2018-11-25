# What's up Github - Issue #6

Hello fellow makers of the web !

Every time I find a cool project, I star it (currently at 896 ⭐️), but I often find interesting things in existing projects, big or small, known or unknown. So I chose to highlight these bits of code.

Last time, I included an interesting Pull Request, and I'm doing it again this week 😎

Please @me on twitter or add a suggestion here if you have nice repos or PR to share. I'd be more than happy to include them here.



[![Artwork By Jono](https://s3.amazonaws.com/revue/items/images/003/827/574/original/twojs.gif?1542608164)](http://archive.jono.fyi/gallery/2018/01-infinity.html).  
by [Jono](https://twitter.com/jonobr1)

🖌 [mattdesl/canvas-sketch](https://github.com/mattdesl/canvas-sketch)

Finally you can combine your passion for art with your passion for code! Generative code is kind of the paint of the programming world. Canvas-sketch is a collection of tools to help you create art with code, randomness, algorithms, and emergent systems. Be it images, audio or interactive canvas. It can be used with your favourite graphics library. The artwork above is made with [twoJS](https://github.com/jonobr1/two.js) by [Jono](https://twitter.com/jonobr1). Behold the new Hopper!

🥩 [sokra/rawact](https://github.com/sokra/rawact)

How do you like your React cooked? Rawact is a babel-plugin that aims to transpile your React components into native DOM operations (similar to [stencil](https://github.com/ionic-team/stencil) and [svelte](https://github.com/sveltejs/svelte)). The idea is to get a faster initial page load by avoiding to download and parse the react and react-dom library. Which you probably don’t need in its entirety to render your initial page. It works by replacing react and react-dom with rawact’s own smaller runtime and `createElement` calls with DOM rendering instructions.

🐘 [graphile/postgraphile](https://github.com/graphile/postgraphile)

How to you put an elephant into a fridge ? You open the fridge, put the elephant in there, close the fridge. Well now, how do you put an elephant into a graph queue hell ? postgraphile. Yeah nonsense.
In short if you want to use GraphQL with your PostgreSQL database, postrgaphile automatically creates and updates a GraphQL server with the right types, columns and relationships. Magic you say ? I’d say PostgreSQL reflection APIs.

🦇 [sharkdp/bat](https://github.com/sharkdp/bat)

Do you remember the last time you `cat` a HTML file and immediately cleared the console, frustrated, because you somehow expected the syntax highlighting to be present ? I don’t, because who uses `cat` these days ? Maybe it’s time for it to make a comeback. Slightly improved that is. Bat has syntax highlighting, git integration, and support for non-printable characters.

☩ [GoogleChromeLabs/ProjectVisBug](https://github.com/GoogleChromeLabs/ProjectVisBug)

Does your product manager checks your grid alignement ? Mine does. I found him this little tool to help him out. VisBug is a chrome extension that allows you to fiddle with the page it’s run on. You can measures spacing, change colors (and all CSS properties), move things around, test for accessibility, edit text, search elements and more. All in a nice UI.

## 🧠 Proposal of the week

🌀 [KenjiBaheux/portals](https://github.com/KenjiBaheux/portals)

The idea of “portals” is to be able to show a page in the context of another page. (like an iFrame) but the difference is that you can activate the inset frame so it becomes the main one, and having the url reflecting the route change. The web has always been browsed with links. Basically not knowing what’s behind it. Portals could come in handy to help with a deeper integration between applications, domains, and websites.
The name Portals is tentative and the proposal is very early stages. Feedback is wanted!

## 🏆 PR of the week

https://github.com/xtermjs/xterm.js/pull/1790

I found this PR digging into the [VSCode](https://github.com/Microsoft/vscode) releases. The editor uses xterm.js for its terminal rendering. Right now, xterm draws on screen thanks to the <canvas> element. The relatively low level APIs allows some performance improvements over DOM rendering by making good use of the GPU. But Daniel Imms seems to think we can get even better performance using WebGL.  
Early benchmarks are showing already good improvements (as much as 900%) regarding the time to draw a frame on screen depending on the size of the viewport.  
To give a scale, as web developers we usually work with the usual 16ms timeframe to draw something on screen to get a nice 60fps rendering.  
The canvas takes an average of 14.81ms per frame while the WebGL version takes 5.4ms/frame on average.
The PR is still at its experimental phase but we could easily see how this could improve rendering of text-based web apps that needs a high throughput.  
WebGL is a cool technology and this is a good way to get started with it.
Thank you Daniel !

