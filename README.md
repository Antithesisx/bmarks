bmarks
======

Store bookmarks in browser-independent .html files.

With [ws](https://github.com/Antithesisx/ws) integration.

### Motivation

Browsers are not good at efficiently keeping track of what pages you have open. Firefox quickly takes up half a gigabyte of RAM, but even the more lightweight browsers can hog your memory. Uzbl takes up about 40 MB of RAM for me.

The solution is bookmarks, but this feature tends to be implemented in a way that does not abide by the UNIX philosophy. For some reason, my personal data is tied to the web interface I happen to use, and I'm forced to see them as inseperable. If I switch between interfaces, I lose the personal data. If I switch from browser A to browser B, that browser must happen to provide a way to import bookmarks from browser A, or I have to start over. This makes switching between browsers difficult.

The purpose of this program is to keep track of your bookmarks in a browser-independent way by simply adding hyperlinks to html files. These files are universal; every browser is compatible.

### Usage

'bmarks-core CATEGORY URL'

This adds a link to URL at the end of CATEGORY.html. The title of the link is the same as the title of that webpage. If the file doesn't exist, it is created.

