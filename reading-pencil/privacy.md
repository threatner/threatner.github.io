---
layout: page
title: "Reading Pencil: Privacy Policy"
description: "Reading Pencil's privacy policy: nothing you read leaves your computer."
permalink: /reading-pencil/privacy/
---

# Reading Pencil: Privacy Policy

_Last updated: 14 October 2026_

Reading Pencil is a browser extension that draws a small pencil under the line
you are reading. This policy says exactly what it does with your data. The
short version: **nothing you read leaves your computer.**

## What Reading Pencil collects

Nothing is collected, sent or shared on its own. Reading Pencil has no
analytics, no crash reporting, no advertising, no accounts and no servers.
It makes two kinds of network request only:

- when you start the pencil on a PDF, or open one from "Where you left off",
  it downloads that PDF from its own address, to show it in a page of its own
  (see "PDFs" below). That request goes only to the website the PDF comes
  from;
- when you write feedback on its feedback page and press **Send**, it sends
  what that page shows to the developer (see "Feedback" below). Nothing is
  sent until you press Send.

## What it stores on your device

Reading Pencil keeps a small amount of information in your browser's own
extension storage (`chrome.storage.local`), on your computer only:

- **Your settings:** your reading pace, Pencil or Line, which hand, color,
  highlight strength, and whether to keep to the article.
- **Where you left off:** for each long page you have started reading with
  the pencil (at most 50; the oldest are removed first):
  - the page's address (for a PDF, the PDF's address; for a PDF you chose
    from your computer, its file name and size, not the folder it is in;
    and, if the site changed its address while you read, up to three other
    addresses of the same article), with tracking
    parameters (such as `utm_source`) and parameters that carry secrets
    (such as tokens, passwords, signatures, session IDs or email
    addresses) removed; very long addresses are not kept at all;
  - the page's title, so the list can show it by name (a title holding an
    email address is not kept);
  - the first 80 characters of the paragraph you were on, used only to find
    that paragraph again when you come back;
  - how far into that paragraph you were (in a PDF, also the page it is
    on), and when;
  - once you have read 20 lines of it with the pencil, a random name for
    that article (made up on your computer, not taken from the page), so
    that reading it again another day adds to the same book on your shelf
    (below) instead of counting it twice.
- **Your reading:** numbers, to show you what you have read with the
  pencil: how many articles, lines and (roughly) words, how long, on how
  many days (with the date of the last), and how many you read to the end;
  and, for your shelf, each article's length in words, whether you finished
  it, and its random name, for at most the last 60. Never which pages,
  sites or words.
- **Whether you have seen the short how-to hint** (a count, so it stops after
  a few times), and **whether you have answered the review question**, so it
  is asked at most twice.

Nothing is stored for pages you read in an Incognito window.

This information is never transmitted anywhere, and websites cannot read it
from the extension's storage. It is used only to draw the pencil, to put it
back where you left off, and to show you your own reading. While the pencil
is drawn on a page, that page's own scripts can see it there (its position
and color, and the "continue" card, the review question, or a note such as
"You've read 10 articles" when one is shown), as they can see anything else
on their page.

## The review question

After you have read three articles with the pencil, Reading Pencil asks
once, at the end of an article or in its toolbar window, whether you would
leave a review (and once more after ten, if you said "Not now"; then never).
If you choose **Leave a review**, it opens the Chrome Web Store's reviews
page for Reading Pencil in a new tab, as a link would. The page you were
reading is not told, and nothing about your reading is sent.

## Feedback

The toolbar window's **Feedback** link opens a page inside the extension
where you can tell the developer what's wrong, or what you'd like. Nothing
on it is sent until you press **Send**. Then these go, through a Google Form
the developer reads (Google's own privacy policy applies to it):

- what kind of message it is, and what you wrote;
- the pages you name: the list starts with the address of the page you were
  on, cleaned as for "Where you left off" (tracking parameters and anything
  that looks like a token, a password or an email address removed, and the
  address cut short where one appears in its path); you can remove it, add
  other links (cleaned the same way) or leave none. Opened from an Incognito
  window, the list starts empty: the private page is not filled in;
- a way to reply, only if you give one (an email address or an X handle);
- a few details that help find a problem, listed on the page under "See them" before you send: the versions of Reading Pencil, your browser and
  your system, your browser's language, your screen's size, whether dark mode
  and reduced motion are on, your Reading Pencil settings, and what the
  toolbar window said about the page (for example "Following 13 lines on this
  page"). Never what you read, your places or your reading numbers.

Your Google account, if you are signed in to one, is not sent with it.

If you remove Reading Pencil, Chrome opens a goodbye page on Reading
Pencil's help site (threatner.github.io), which asks why, if you'd like to
say. Its address tells the page the version of Reading Pencil you had and
your browser's name and version. Nothing is sent unless you press Send
there; then what you chose and wrote, with that version and browser, goes
to a Google Form of its own (not the feedback form), and nothing else.
The page has no analytics and sets no cookies.

## PDFs

Chrome's own PDF viewer lets no extension in, so when you start the pencil on
a PDF, Reading Pencil opens it in a page of its own, inside the extension. To
do that, it downloads the PDF from its own address (the one your browser
opened, or the one kept in "Where you left off"), with your browser's cookies
for that website, as your browser itself would (so a PDF you had to sign in
for still opens). The PDF is shown and read on your computer. It is not
stored, and it is not sent anywhere else. A PDF you choose from your computer
is read from that file and never leaves it; your place in it is kept by its
name and size, so choosing the same file again takes you back to your line.
PDFs are not opened from Incognito windows.

## How to remove it

- Open the toolbar popup → **Where you left off** to forget one page or all of
  them.
- Uninstalling Reading Pencil removes everything it stored, your reading
  numbers included.

## Permissions, and why

- **Read and change data on websites** (content script and host access for
  `http` and `https` pages): when you start the pencil on a page, to find the
  text of the article and draw the pencil over it; and when you start it on a
  PDF, to download that PDF from its own address and show it in Reading
  Pencil's page. Page content is read in your browser to measure lines; it is
  never stored (apart from the 80-character excerpt above) or sent anywhere.
  The same access lets the feedback page send your message to the
  developer's Google Form when you press Send.
- **storage:** to keep your settings, your places and your reading counts on
  your device.
- **activeTab** and **scripting:** to place the pencil on a tab where it
  isn't running yet, when you ask for it there; and once, when the extension
  is installed, updated or switched back on, to give the web pages already
  open its script, so that "Start reading here" works in them without a
  reload. Until you start the pencil, that script only notes where you
  right-click, and, when you open the toolbar popup, counts the lines it
  could read there. Nothing leaves your browser.
- **contextMenus:** the "Start reading here" item in the right-click menu.

## Children

Reading Pencil collects no data from anyone, including children, apart from
feedback someone chooses to send.

## Changes

If this policy ever changes, the new version will be published here with a
new date. Reading Pencil will never begin collecting or transmitting data
without a new version of the extension and of this policy.

## Contact

Questions: message [@threatner_ on X](https://x.com/threatner_).
