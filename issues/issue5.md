# What's up Github - Issue #5

Hey everyone !

Quite a few of you just joined the wagon in the last few days. Keep ‘em coming. Share and give feedback on [twitter](https://twitter.com/dot_louis) or on my [feedback board](https://whatsupgithub.nolt.io).

But let’s see what’s up on github this time:
_No I won’t talk about react hooks. I promise._

![You either love that yellow or you hate it.](https://s3.amazonaws.com/revue/items/images/003/753/709/mail/30791512-cb001438-a167-11e7-952b-f0f0e5c4499e.png?1541347287)

🎨 [dawnlabs/carbon](https://github.com/dawnlabs/carbon)

I bet you’re the type of person who posts 👏 [his](https://twitter.com/notquiteleo/status/873483329345028096) 👏 [code](https://twitter.com/reactjs/status/890511993261654017) 👏 [online](https://twitter.com/dot_louis/status/1022425816418926592) 👏. Don’t fret, we won’t judge your editor color-scheme. Jk I will.

Someone wants to help you. Carbon lets you create beautiful images to share your code with style or to set as the desktop background of your non-tech friend to see him jump scare.

🐨 [nuxt/consola](https://github.com/nuxt/consola)

It’s been a long time since logs in JS haven’t been dusted. Since the days of [Bunyan](https://github.com/trentm/node-bunyan) and [Winston](https://github.com/winstonjs/winston). The [Nuxt team](https://nuxtjs.org) is coming with a new module to handle it. They promote:

- Easy to use
- Fancy output with fallback for minimal environments
- Pluggable reporters
- Consistent command line interface (CLI) experience
- Tag support
- Redirect console and stdout/stderr to the consola and easily restore redirect.
- Browser support
- Pause/Resume support
- Mocking support

To be fair I haven’t tested it but … that koala is dope tho.

![From: a martian who wants you well](https://s3.amazonaws.com/revue/items/images/003/753/800/mail/example.png?1541349363)

👽 [ai/size-limit](https://github.com/ai/size-limit)

Apparently some martian folks care about us. Or rather they care about the size of our bundles. They developed a small tool to keep that size in check.

You simply npm install it then specify a limit for your bundle not to reach. You can set this up in a CI environment to make it throw an error when exceeding the limit. The little touch I like:

Specify `–why` in the command line and you will be shown the truth. Or at least the details of what dependency is taking up that much space.

🕶 [matiassingers/awesome-readme](https://github.com/matiassingers/awesome-readme)

**Readme.md**. You love to read that file. But oh you hate writing it! Writing a good Readme is vital to get your project adopted and shared, but how do you do it ? What section should you include?

Now you have great examples to get inspired from. There are also tools to help you get started, make screen records of your terminal and more. You can even ask for feedback on your own !

🏅 [FiloSottile/mkcert](https://github.com/FiloSottile/mkcert)

If you’re are using Service Workers. You know those can only be used with **https**. (I think you can bypass this requirement with the chrome devtools). But in general working on **localhost** doesn’t rythme with https. Mkcert automatically creates and installs a local CA in the system root store, and generates locally-trusted certificates.

I literally had `https://localhost:3000` working in 20 seconds with it.

## 🏆 PR of the week

https://github.com/prettier/prettier/pull/5259

You should all know [Prettier](https://github.com/prettier/prettier) by now. If you don’t… well, there is a whole new world of productivity waiting for you just behind that link.

Since I began using Prettier, there is not a single project I start without `npm i prettier` first.

Your Js(x), Ts(x), Json, GraphQL, CSS, Markdown… made beautiful in an instant. The elephant in the room was the missing support for HTML.

Structuring HTML is a lot harder that JS, mainly due to the meaning of spaces in the language. The same way JS can be minified pretty easily, HTML not so much.

Rules must have been set. And as usual, prettier is opinionated. So you may not like its way of formatting things. But I feel that we should not care anyway. Consistency and not having to think about indentation beating formatting preferences any day.

So big thanks to [ikatyang](https://github.com/ikatyang) for championing this huge PR !
