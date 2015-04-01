---
layout: post
title: Reliance On Web Applications
cover: cover.jpg
---


Every day, features of traditional websites approach
those of stand-alone desktop programs. Strictly informational websites
with simple indexes and content still have their place on the web and
they probably will continue for a long time, but this post isn't about
that. Commonly called web-apps, they often offer only a few actual
"pages"(typically there are no true page changes once you're logged in,
the page is simply redrawn to make it appear as though there is page
navigation). These web-apps maintain state, redraw their user-interfaces
(sometimes with
animations), have multiple threads running in parallel and behave like
stand-alone desktop applications in just about as many ways as you can
think of. We see these web-apps vying with their native application
competitors for market share, performance, ease-of-use, features and
reliability among many other things. An example is the comparison of the
Google Drive suite with the Microsoft Office Suite or Libre Office. In
fact, Google's offering of their Chromebook laptop whose operating
system's  window manager is quite literally a web browser is the
most telling example of exactly how far this trend can be taken. On
those devices quite literally "everything" is done and runs within in
the browser. The main reasons why some choose to utilize these web
applications over a native application include the following:

1. Ease of access. Everyone has a browser, everyone knows how to type a
URL into their address bar.
2. Perceived security. Visiting a website ought to be safer than
downloading a full-fledged application which will be installed into the
operating system. Presumably the browser can safely "sandbox" the code
and minimize any damage that it might try to wreck upon my computer or
other browser tabs.
3. Convenience. All activity seems to be synced quite well into the
**cloud** and are available wherever I can access my user account on a
browser.
4. Exclusivity. The software isn't available as a stand-alone
application to be installed into the operating system, thus the user has
no choice if they wish to utilize the feature set which the app offers.

As an extra aside, a software developer might choose to develop their
next great software idea as a web-application rather than a standalone
desktop application simply because it's typically much less work to do
so and the resultant program will be in essence functionally equivalent.

I like to use myself as the first example whenever possible. So I'll
begin by listing the web-apps I find to be most useful to my own workflows.

1. Trello. It's a free online whiteboard for stickies and post-its- on
drugs. To-date I haven't found an organizational took like it. Whenever I
have a new idea I'm often overwhelmed about where to begin. Enter Trello. I
create a new board with a title of the idea "Solve World Hunger" and
begin creating lists and cards to organize my plan of assault. It's also
trivial to add collaborators into the mix so that I can organize with my
colleagues or partners.
2. Gmail / Google Inbox. This is much more than just an e-mail access
portal. I believe Gmail's browser offering fits the profile of a
full-fledged email client.
3. Github. It's the best and easiest graphical Git client/visualization
tool that I know of. There are others that come close. (See Atlassian
bitbucket, I use this also because it's cheaper to host private
repositories).
4. NewRelic Server and Application monitoring.
5. Google Drive & Office Suite
6. Soundcloud

The only true initial upfront cost of these applications is bandwidth,
at least at face value. However I think it's worth noting a few
considerable drawbacks when it comes to using a web-application.

The first is security. In a nutshell when you use a web-app, your
browser requests a page from a computer somewhere else on the planet
that is also connected to the internet. Let us use the example of Gmail.
You begin by typing `https://gmail.com` into your browser. Your browser
fires a request off to Google's servers for the web-page and code that
make up that webapp.
Presumably Google receives the request and sends you back the data you
requested. The assumption here is that your request did genuinely make
it to Google's servers and the response has not been tampered with in
any way. Anything short of this, and you could actually be receiving a
modified version of gmail's web-app that likes to eavesdrop on all of
your emails, or record your password or worse. There are techniques for
mitigating the
risk of such attacks (and this is just one simple vulnerability, there
are numerous) but there aren't very many guarantees for security with
this model.

Another bottom line is that all your precious private data lives in the
cloud and you're just going to have to trust that it's being stored in
the most secure ways possible and that even the threat of a disgruntled
employee on the inside of the web-app provider's organization is
non-existent.

The next major drawback I see within web-apps has to do with data
retention. If you use these services as often as I do, you begin to
accumulate a lot of stored data. Emails, documents, bank statements,
organization lists, digital media and everything in between. You then
begin to wonder what measures the service provider has taken to reduce
the possibility of precious data loss. Then, assuming they've left no
stone unturned to ensure that every single byte is accounted for, what

if they go out of business or otherwise fall off the face of the planet?
There seems to be no standardized way to keep a backup of the data
stored therein and it seems like that's just too much trust to place in
the hands of these entities.
