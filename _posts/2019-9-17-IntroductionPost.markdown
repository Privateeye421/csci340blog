---
layout: post
title:  "Introduction Post"
date:   2019-09-17 19:27:11 -0500
categories: jekyll update
author: Jack Frey
---
Considering how awful I am at installing files any more complex than a download button, everything went pretty smoothly! I've never
actually used the command line too extensively, so a lot of how it works was new to me. I figured it out pretty quickly, though.

I only had problems with a few things:
* I had trouble getting my cmd to see Ruby as a valid command.
* I also had trouble getting the bundle installer to find my Gemfile.
* Once I had Jekyll installed, the blog setup command wouldn't work.

For the first problem, all I had to do was restart cmd, as found [here][helplink1]. For the second problem, I ran bundle init,
which created a new Gemfile that the program did read, as suggested [here][helplink2]. For the third one, Ruby itself suggested
I rerun "bundle install", which fixed the problem. I'm really not sure why I had to run bundle installer twice to get the whole
thing to install, but at least it worked. I've never really had my own blog before, so this is a really cool idea!

[helplink1]: https://stackoverflow.com/questions/15822686/why-is-ruby-not-recognized-as-an-internal-or-external-command/34956453
[helplink2]: https://stackoverflow.com/questions/50596235/could-not-locate-gemfile-even-though-bundler-is-successfully-installed
