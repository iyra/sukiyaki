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

### Update (2020-03-03)
maki64 has kindly added proper credit to my project in their README for
makiba (https://github.com/maki64/makiba).
