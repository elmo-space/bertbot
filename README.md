# bertbot

#### stupidly easy IRC bot written in python(3)
I wrote this bot over the course of the last year. It grew and new function were added every now and then.<br>
The code is pretty ugly and the bot has some serious problems with memory leaks and random disconnects and lacks an automatic rejoin function.

But overall it is a pretty fun thing and is heavily used on the IRC server that I am currently using (n0xy.net).

##### some of the available commands (mostly funny useless shit):
|command|action|
|-----|-----|
|.nextrocket|shows the next upcoming rocketlaunch (data from LaunchLibrary)|
|.slap|slap a user (similar to the slap command of mIRC)|
|.rep (\<reason\>)|super simple reputation system. you can give an optional \<reason\>)|
|.eurusd|convert euro to usd|
|.usdeur|convert usd to euro|
|.jn question|choose between yes or no|
|.twitter account|get the last tweet of \<account\>|
|.trump|get trumps last tweet|
|.konfuzius|get a konfuzius quote (in german from wikiquote)|
|.say \<message\>|make the bot say something (only for admin user)|
|.fml|get a random fml from fmylife.com|
|.nslookup \<domain\> (\<type\>)|make a dns lookup for \<domain\> with optional \<type\>|

##### automatic triggers
- All http links are parsed and the html title is printed out if one is found
- The bot automatically parses all twitter links and prints out the full tweet and account name.
- The blog of the german blogger "fefe" (Felix von Leitner - blog.fefe.de) is crawled every five mins. and new Posts are automatically printed out with a link to the post
- eFukt is crawled every 10 mins. and a message is generated on new videos (it also triggers another bot in our network)
