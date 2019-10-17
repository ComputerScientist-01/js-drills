# Pineapple Curry

Toy problems and drills!

There's a reason for this repo's name.

## JS and CSS

Possible solutions are included in the same files as the questions,
after long empty comments. Don't jump to the bottom and cheat!

## Node and Express

* There _will_ be things in here that are completely unfamiliar. I strongly suggest
  keeping [this](https://nodejs.org/api/) open at first.
* There's a directory of bare Node (no Express/Koa/Hapi/whatever framework) problems.
* There's a handful of Express drills.
* You'll touch on ES2015 going through these. It's time to exercies your Googling skillz!
  * Read up on `let`, `const`, and arrow functions.
  * You may need to upgrade Node. I highly recommend using `n` for this.
    * `npm i -g n ; n latest ; npm i -g npm@next` (might as well get the cool new features!)
* Remember that programming in Node should almost always be done asynchronously.
  * `require`s are synchronous; almost everything else should be using callbacks.

Here's an example of a very simple Node program, using modern ECMAScript.

```javascript
'use strict'

const port = process.argv[2] || process.env.PORT || 5678
const { createServer } = require('http')

createServer((req, res) => {
  res.end('hi', 200)
}).listen(port)
```

This is a lot of new material all at once. Do what you're comfortable doing.
If you're looking for something to do over interim week, maybe do some research
and try to finish the rest.

Have fun!

## React

* For the moment, just imagine there's an `index.html` with a div you can target,
  and your build system is already taken care of for you.
* [WebpackBin](http://webpackbin) is a good environment for testing out React ideas
  (it's like a JSBin that lets you use modules).

## Contributing

PRs, issues, and suggestions welcome.

If contributing code, please ensure you are following the editorconfig and eslintrc.
Your code will be reformatted if not.
