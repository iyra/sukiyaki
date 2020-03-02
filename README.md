A futaba-style imageboard script that doesn't require a database.

To install, move all the files in the repo to a directory in the
root of your webserver. For example, for a board called `/jp/`, move
them to /usr/share/nginx/html/jp/. Create the directories `src`,
`thumb` and `res` and the file `posts` and make sure they are all
writable to by the web server user.

Should work on any unix-like system with PHP 5.5 or above.

Protip: you can use it as a blog too, by setting the following:
```
ADMINOPONLY=1,
SORTBUMP=0
REPLYBOX_TOP=0
SHOWPOSTLIST=1
PERPAGE=1 if you want
```
## My code was copied(?!)

Now for the drama. This code was originally released under the public domain.
I'm usually very open with peolpe copying my code, and making any changes
that they wish to. However, I realized that the tripcode generator function
that I'm using is under the GPLv3. That license mandates that I change the license
to my own code to a compatible license. I re-licensed to the GPLv3 (see the
commit history).

Around the beginning of 2020, after I re-licensed under the GPLv3, someone on
Github called "maki64" copy-pasted my code, verbatim - and only added a bit of CSS at
the top of the file. This happened on 27th Jan[0]. The only other change maki64
made in the commit was to change the contents of the footer to read "makiba", the
name of his/her "own" script, "makiba".

Makiba came to my attention on 2020-03-02, when I was browsing the Wikipedia artcile
page for imageboards. "makiba" is listed there, with a link to maki64's repository
of the same name. Naturally, I was curious as to how maki64 implemented flat-file
storage. To my surprise, all of the code in his "post.php" (formerly my "sukiyaki.php")
was copied from me. Several changes were made over time, including the reference
to "sukiyaki.php"[1]. The instructions in my README and description of my script
were also copied verbatim.

This wouldn't be a problem usually, except for the fact that on the initial commit,
I wasn't credited - in any way. Even when maki64 added a README, I wasn't credited
initially[2]. This is to say nothing of the fact that as of this update to my README,
makiba is in violation of the GPLv3, unlike my own code. Even if maki64 had used
the public domain version commit of my code, that would not change the fact that
someone else's tripcode function is still in maki64's code, and would require the
license to be GPLv3.

On 2020-02-07, a line in the makiba README was finally added to show I had something
to do with the project (such has having written all of the code...), though apparently
only "half" the code, despite the meager additions from other contributors to the
makiba codebase. Later on, on 2020-02-09, they simply changed it to say that
my code was "made better :^)"[4]. My Github username was not mentioned, only "sukiyaki"
which is the name of my script. Other contributors were mentioned by name, and I
was not. I suspect this has something to do with the fact that maki64 didn't want
many people finding out that I wrote the code.

I went to the makiba Discord[5], with around 30 members, server to relay my concerns:
![My post to their chat server](https://i.imgur.com/nGkVmcx.png)

Despite my cordial tone and offer to help, I received no response and was instead
permanently banned from the Discord chat.

The fact that makiba is in violation of the GPLv3, and the rude way I've been treated,
I cannot recommend that anyone use makiba. I don't regret my decision to release
the initial version under the public domain, but my faith in Github users has
been lessened by the fact that no thought was given to the original author of
the code. maki64 even went to the length of claiming that the code was written
"from scratch" by themselves on 4chan's /qa/ board[6].

I recommend you use another PHP imageboard software, with more features than both
my own, and makiba - and we can leave a project that doesn't give due credit and 
treats contributors so unkindly to die.

Below, I have included references to a forked edition of the code on my own
Github account, lest maki64 moves "their" code elsewhere.

[0] https://github.com/iyra/makiba/commit/1ae19620fa1d5c303808c46ca3a7ff1eead1a209

[1] https://github.com/iyra/makiba/commit/ec108c8973ee6169bad258d0c62b214f2e2dedd4

[2] https://github.com/iyra/makiba/commit/37c12481455f376bbdf7bb32d6b82caa9bcd549a

[3] https://github.com/iyra/makiba/commit/1ed39e336b0138cd817eef57b7983bc009372a93

[4] https://github.com/iyra/makiba/commit/d4bf0e464adfc3a214cb0ab5770bda132d93d680

[5] The chat was active for a while. Here's a screenshot of maki64 and others trying
to figure out how to use my code: https://i.imgur.com/3xm8PsG.png

[6] https://desuarchive.org/qa/thread/3114538/
