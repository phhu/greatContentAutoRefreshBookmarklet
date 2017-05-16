# reloadAndBeepOnChangeBookmarklet
A bookmarklet used to create a beep when new jobs appear on supertresc.pl / greatcontent 

This is useful because it saves having to manually refresh and monitor the page for new jobs: you will hear a beep when new jobs appear, and can take them promptly.

Installation
============

Go to https://cdn.rawgit.com/phhu/reloadAndBeepOnChangeBookmarklet/master/installationLink.html and drag the link on that page to the bookmarks / favourites bar.

Alternatively, create a new bookmark and put the contents of file ```reloadAndBeepOnChangeBookmarklet.js``` as the URL. 

Use
===

Once on the main page, where job listings appear, click on the bookmarklet on the bookmarks bar / menu / folder. It will prompt for a refresh interval in seconds, and thereafter will refresh the page on that interval.

You can monitor its function by opening developer tools (ctrl-shift-J in Chrome) and looking at the console.

Workings
========

It reloads the page at specified intervals and looks for an increase in the number of table rows in the content div. If there is an increase, a beep sound is emitted three times. (It therefore won't handle a job being replaced by another such that the count remains the same, but this is a rare case!)
